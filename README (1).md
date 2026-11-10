# Post-mortem: UniV3-family vault exploit, 2026-11-08

## Post-mortem: UniV3-family vault exploit, 2026-11-08

**Status:** mitigated. Every affected vault has rejected deposits since 16:40 UTC on Nov 8, and that is verified on-chain. Withdrawals remain open.

**ACryptoS is being deprecated.** No fix or re-opening of deposits is planned. Users should withdraw their funds.

### 1. Summary

The ACryptoS concentrated-liquidity vaults (UniswapV3, SushiswapV3, PancakeSwap v3, Biswap v3) accepted a `depositMulti` call whose `_amounts` array was **shorter than the vault's token count**. With a 1-element array, the vault priced _its own holdings_ using only token0. So a small token0-only deposit minted most of the vault's shares, and an immediate `withdrawMulti` paid out a pro-rata slice of **both** tokens.

From 02:02 to 16:22 UTC, **135 addresses** exploited this across **5 chains**, extracting about **$665k**. A beacon upgrade disabling deposits went out on all 11 beacons between 15:38 and 16:40 UTC, and exploitation stopped on each chain as its upgrade landed.

### 2. Impact

USD values use prices from 2026-11-08 \~17:00 UTC (ETH $2,226, BTC $75,662, BNB $695, XSGD $0.78, OP $0.10; stables $1). They don't include about 19.4k ACS taken from the BSC ACS/WBNB vault, which wasn't priced.

| Chain     | Vaults hit    | Exploit window (UTC) | Extracted      |
| --------- | ------------- | -------------------- | -------------- |
| Arbitrum  | 28 of 40      | 02:02 – 15:53        | $230,213       |
| BSC       | 12 of 33      | 04:22 – 16:19        | $190,845       |
| Polygon   | 11 of 16      | 05:45 – 15:38        | $134,686       |
| Base      | 13 of 18      | 07:02 – 15:11        | $69,813        |
| Optimism  | 13 of 16      | 07:31 – 16:22        | $39,871        |
| Linea     | 0 of 3        | –                    | $0             |
| **Total** | **77 of 126** |                      | **≈ $665,429** |

The losses fall on honest depositors in each vault. They were diluted by the over-minted shares, and their tokens were paid out to the exploiters.

### 3. Root cause

`depositMulti(uint256[] amounts, uint256 minShares)` did not check that `amounts` had one entry for each of the vault's tokens. With a single amount on a two-token vault:

* the deposit was valued using token0 only, which is correct for a token0-only deposit;
* **the vault's existing holdings were also valued using token0 only**, ignoring everything it held in token1.

If the vault held little token0, for example an out-of-range position sitting almost entirely in token1, even a tiny deposit was worth a multiple of "the vault" and minted most of its shares. `withdrawMulti` then paid those shares out pro-rata over **both** tokens.

Pool prices were not manipulated. The flaw had been present since these vaults were first deployed; no recent upgrade introduced it. Every vault in the family was affected.

#### Fork proof

Polygon fork at block 96940861, just before the first deposit on the Polygon USDC/USDT0 vault `0x61A3…874D`:

```
vault before: 4.958349 USDC / 72,825.21 USDT0
depositMulti([10000000])    -> 118,644,929,973 shares = 66.84% of supply   (on-chain mint: 118,644,929,973, an exact match)
depositMulti([10000000, 0]) ->       8,087,968 shares =  0.01% of supply
round trip: in 10 USDC, out 9.989999 USDC + 48,634.255398 USDT0          (matches on-chain tx 0x28d620b2…)
patched implementation: depositMulti reverts "deposits disabled"
```

Attacker calldata for tx `0x80cc054f…`: `depositMulti([10000000], 0)`.

Across all chains, **\~1,000 deposits** were classified by decoding their calldata: an amounts array shorter than 2 is the exploit signature. A further \~220 deposits went through attacker contracts or EIP-7702 delegated wallets and were counted by their net profit.

### 4. Attack walkthrough

Each round is two transactions about 1–2 minutes apart:

1. `approve(token0)`, then `depositMulti([small token0 amount], 0)`. This mints most of the vault's shares.
2. `withdrawMulti(allShares, false, [0, 0])`. This pays out the deposit back plus most of the vault's token1, less a 0.1% withdrawal fee in shares.

Each round removes a constant fraction of what's left in the vault. That's why the first Polygon vault lost 67%, 67% and then 90% of what remained in successive rounds.

### 5. Timeline (UTC, 2026-11-08)

| Time           | Event                                                                                                                  |
| -------------- | ---------------------------------------------------------------------------------------------------------------------- |
| 01:50          | `0x5dc8…f322` funded with 12.98 ETH on Arbitrum through a **Mayan Swift** cross-chain order (`SwiftDest.fulfillOrder`) |
| **02:02**      | **First exploit**: `0x5dc8…` on Arbitrum WBTC/WETH-500                                                                 |
| 04:22          | First BSC exploit, `0x8232…a5d2` (BTCB/WBNB-500)                                                                       |
| 05:45          | First Polygon exploit, `0x6485…49f` (USDC/USDT0-100)                                                                   |
| 07:02 / 07:31  | First Base exploit (`0xa597…261d`) / first Optimism exploit (`0x706f…`, via contract)                                  |
| 07:50 – 09:50  | `0x6485…` bridges 51.85 WETH from Polygon to Ethereum via Across                                                       |
| \~09:30 onward | Copycats: 100+ addresses, many of them EIP-7702 wallets running identical one-shot rounds on every chain               |
| 09:34          | Exploit first reported to the project on Telegram                                                                      |
| 14:19          | Developer notified                                                                                                     |
| 15:38:58       | Polygon UniV3 beacon upgraded (last Polygon exploit 15:38:46, 12 s earlier)                                            |
| 15:56 / 16:04  | Arbitrum UniV3 / SushiV3 beacons upgraded                                                                              |
| 16:20          | BSC UniV3 upgraded                                                                                                     |
| 16:23:49       | Optimism upgraded (last exploit 16:22:27)                                                                              |
| 16:27 / 16:29  | Base UniV3 / SushiV3 upgraded                                                                                          |
| 16:30          | Linea upgraded (never exploited)                                                                                       |
| 16:38 – 16:40  | BSC PancakeSwap / Biswap / Biswap2 upgraded; all 126 vaults closed                                                     |

Since then, a full scan of every vault shows **0 successful deposits** after its upgrade, and every beacon still points to the patched implementation. Nov 1–7 had no exploit deposits on any chain: Polygon, Arbitrum, Optimism and Base were checked for the whole week, and BSC for Nov 7.

### 6. Exploiters and fund flows

| Address                                      | Extracted           | Chains         | Notes                                                                                                                                                                                                                                                                |
| -------------------------------------------- | ------------------- | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `0x5dc8df8d0d6cfae0443bb8d9eacdfbb72b2ef322` | $139.5k             | Arbitrum       | Started first. Funded through Mayan Swift. Swapped through 0x `AllowanceHolder` and Uniswap; bridged out through **Mayan** (`MayanForwarder2`: 45,754 DAI + 22.4 WETH + 14.06 ETH), **Squid**, **Relay** and the **USDe OFT** (LayerZero)                            |
| `0x648508c5e95e7c9ac2380672f87d60ebb1dae49f` | $111.8k             | Polygon        | 72,019 USDT0, 13,178 XSGD, 12.9 WETH and 831 DAI swapped to WETH (Velora/ParaSwap and other aggregators), then **51.85 WETH bridged by Across to Ethereum, to the same address**. **It still holds 50.82 WETH (≈ $113k) on Ethereum.** Address active since May 2026 |
| `0xcafe343896335dde2d36a43c85395fd93d659956` | $84.7k (+10.5k ACS) | all 5          | 162 rounds. Uses the same 0x `AllowanceHolder` `exec` pattern as `0x5dc8`. Splits proceeds to look-alike vanity addresses (`0xcafedc6c…`, `0xcafe8f02…`, `0xcafeaedd…`), which are also exploiters                                                                   |
| `0x82328b24ed97d6e627b6257d125cb3271c5aa2d5` | $80.5k (+8.9k ACS)  | BSC            | **Still holds 116.5 WBNB (≈ $81k)**                                                                                                                                                                                                                                  |
| `0x2143a65fc4721aea20b4ebf99e775b1e6cc9a1a7` | $54.2k              | BSC            | **Still holds 78.2 WBNB (≈ $54k)**                                                                                                                                                                                                                                   |
| `0xa5970e20d011a1c8406bbf9315389f6d831b261d` | $49.6k              | Optimism, Base |                                                                                                                                                                                                                                                                      |
| `0x00aa588bbb6f48005198b6d4a699107542566970` | $37.6k              | 4 chains       |                                                                                                                                                                                                                                                                      |
| 128 others                                   | ≈ $107k             |                | 28 addresses each hit ≥3 chains with identical one-shot rounds, $243k between them, which suggests a shared script                                                                                                                                                   |

**Freezable stablecoins still in exploiter wallets: under $1k in total** (USDC/USDT dust). The rest was swapped to ETH/WETH/WBNB or bridged.

**Where to send freeze or tracing requests:** Mayan (orders funding and draining `0x5dc8`), Across (`0x6485` deposits to Ethereum), Squid/Axelar, Relay, LayerZero/Ethena (USDe OFT). The three wallets still holding WETH/WBNB should be watched and flagged to exchanges.

### 7. Response

* Once the developer was notified, the first chain was closed in 80 minutes and all chains within 2h21m, with one beacon upgrade per vault family. No per-vault transactions were needed.
* Each chain was dry-run on a mainnet fork before going live, and each upgrade was verified on-chain afterwards.
* The fix also auto-pauses each vault on its next transaction, so leftover liquidity is pulled out of the pools.

_Method: on-chain logs, receipts and calldata via public RPCs and the Etherscan v2 API, plus a Hardhat mainnet fork for the proof. Scripts are kept locally and are available on request._



### Update 2026-11-09: Base DAI/USDbC vault restored

One exploiter still held 99.99% of the Base DAI/USDbC-500 vault and began draining it on Nov 9. We upgraded the vault ([`0xff8b639b…`](https://basescan.org/tx/0xff8b639bb055cfc4a420aca7393c6664248ab47ebbc5ec52179caf79403f9d39)) and burned the exploiter's shares and the excess fee shares minted after the exploit ([`0x6f2aee72…`](https://basescan.org/tx/0x6f2aee72e13f823f43cd554832270c8b218960522ff2a2f11d6d7693db8a1941), [`0x61e269b9…`](https://basescan.org/tx/0x61e269b9b39de5a8372a02f8c18da18a5d28f31d363646beae073a1f942f9c06)).

The share supply is back to its pre-exploit value. About 1,800 USDbC was lost before the burn. The remaining **6,187 USDbC is withdrawable pro rata by the original depositors.**
