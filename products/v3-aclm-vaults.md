# ACLM
**Advanced Concentrated Liquidity Manager**

Our ACLM is built on top of V3 Conc. Liquidity DEXs (namely UniswapV3 and its forks). Using uniquely developed strategies, we improve swap rate efficiency for liquidity pairs (less slippage), and we achieve a higher than average APY for users providing liquidity. 

Key features of our ACLM include:

- Dynamic setting of positions and ranges.
- Automated rebalancing for optimal yields.
- Simplified single-token deposit system.
  
Our Strategy automatically compounds fees and rebalances its position around the current price. This streamlines the liquidity provision process, reducing additional actions from users, earning them sustainable yields via swap fees.

### Concentrated Liquidity - A Quick Look

How conc. liquidity works is by letting users be strategic about their liquidity provisioning. Instead of spreading your assets across the entire price range, you can choose a specific price zone to focus on. This allows you to earn higher fees on trades that happen within your chosen zone.

**Caveat:** While concentrated liquidity offers much higher APY when trades happen in your set range, it also comes with trade-offs. Once trades move outside your chosen price zone, there will be zero fees rewarded, and extreme price movements can lead to imbalanced positions and impermanent losses that are much higher than V2 LPs.

A detailed understanding of V3 Concentrated Liquidity can be found [here](https://docs.uniswap.org/concepts/protocol/concentrated-liquidity) in Uniswap docs.

## How our ACLM stands out

Our ACLM distinguishes itself from other liquidity managers by maintaining a dynamic range on V3 positions, adjusting to be narrower or wider depending on price fluctuation and volatility trends. This approach ensures that we consistently manage to host active liquidity, leading to more efficient swap volumes.

Our Vault strategies strive to maintain very tight positions around stable / pegged pools (e.g. 1-tick / 0.01% range on USDC/USDT), and wider rages on more volatile pools.

**Examples of past performance:**
- Stable vaults delivering consistently strong yields over a number of months, eg.
   - USDC/DAI at 20-30+% APY  
   - wstETH/ETH at 10+% APY  
   - WBTC/BTC.b at 10+% APY 
- High-yield returns on volatile pairs, successfully countering impermanent losses, eg.
   - ARB/ETH at 101+% APY
   - BTC/ETH at 36+% APY
**the above APY are all achieved purely via swap fees*

- Dominating over 90% of active liquidity in OP Chain's USDT/DAI and USDC/USDT pools ([link](https://app.acryptos.com/u3i/pools/10/0xF1F199342687A7d78bCC16fce79fa2665EF870E1/?a=0x9F0d1DB674488eaF2DE5fd722176CD751803fEf5))
- Hosted 20%+ of active liquidity in OP Chain's wstETH/ETH pools
- Hosted 50%+ of active liquidity in Base Chain's USDC/USDbC pool

![Screenshot of managed USDT-DAI (Optimism) active liquidity %](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/u3i%20-%20Optimism%20USDT-DAI.jpg)
**managing 88.3% of active trading liquidity for USDT/DAI Uniswap V3 (Optimism) - 28 Feb '24*

In comparison with other concentrated liquidity managers, our strategies have outperformed in yield generation for the exact same pools managed. Attached below is a [historical chart](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/History%20-%20Arbitrum%20USDC-DAI.jpg) for the yields generated by our managed USDC-DAI pool on UniswapV3 (Arbitrum) for the period of 18 Dec '23 to 18 Jan '24

- 3.13% yield in 30 days
- potentially extrapolated to 38.08% APR

![History of yields gained for USDC-DAI (Arbitrum)](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/History%20-%20Arbitrum%20USDC-DAI.jpg)

## Understanding the Source of APY

Many defi users that have been depositing in V2 LPs may be familiar with the farming mechanism, where staking an LP gets you APY from DEX farming tokens.
APY from V3 Conc. Liquidity pools comes mainly from swap fees, providing a sustainable source of yield for liquidity providers.

Some additional APY are added as incentives via Merkl. Our vaults are designed to harvest the rewards and compound them for users automatically.

## UI Explanations

The following explains sections of the UI, showing detailed info about each of the vaults.

### Vault Header APY

APY displayed on the header is pulled from the last 8th compound of the vault. (see below)

![Vault Header APY](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/ACLM%20-%20Vault%20Header%20APY.png)

Expanding the "Advanced" section, you can find a table displaying the Historical APY of this vault
"180%" can be seen from the 8th row (3rd column) - Cumulative

### Historical APY

![Historical APY](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/ACLM%20-%20APY%20History.png)

Explanation of the Historical APY:

- Each line refers to one of the latest rebalancing/compounding
- For the 8th line, it can be explained as:
  - the compound was 1.05 days ago
  - the APY achieved between 0.96 - 1.05 days ago is 149%
  - the Cumulative (Total) APY achieved between now and 1.05 days ago is 180%
  - the Impermanent Loss (IL) between 0.96 - 1.05 days ago was -24%
  - the Cumulative IL between now and 1.05 days ago is positive 0.64% (gains instead of IL)

### Chart - u3i
We have developed a chart to help users visualize the current distribution of liquidity on a specific LP, the current trading price, and the active liquidity managed by our strategies.

Expanding the "Advanced" section under each ACLM vault, you can find a "u3i" link.
![Screenshot of managed USDT-USDC (Arbitrum) active liquidity %](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/u3i%20-%20Arbitrum%20USDT-USDC%20240228.png)
- blue bar indicates managed liquidity on ACryptoS
- grey bars indicate other providers
- large amount of under-utilized liquidity can be seen from the grey bars

### Graph - History

Expanding the "Advanced" > "History" section, you will see a graph indicating the historical performance of this ACLM vault.

![History Graph](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/History%20Graph%20-%20VELA-ETH.jpg)

The above is a graph for the VELA/ETH vault on Arbitrum Uniswap V3.
- blue line is the APY gained
- cyan line is the IL
- green line is the nett APY

To understand this graph, we look at the green line to find out the actual APY received.
- the graph shows a period from 18 Nov to 4 Dec 2023
- Green lines shows 27.12% gained from 18 Nov to 4 Dec (18 days)
- Converted to APR 27.12% / 18 days * 365 days = 549%
- Converted to APY = 23155%

**The history graph pulls data from the last 188 harvests of the vault.*

## Exploit Risk Mitigations

The multi-token nature of the vaults and their auto-rebalancing feature on concentrated liquidity AMMs make them vulnerable to price manipulation/flash loan type attacks. We have implemented some mitigations to address this:

* We use historical TWAP to detect price volatility / manipulation, which pauses Vault functionality.
* There is a cooldown period after every vault rebalance, which pauses Vault functionality.
* Deposits and withdrawals are subject to slippage checks. Users should check and confirm the correct amounts to be received on the UI before signing transactions.

The risk of attacks increases as Vault TVL forms the bulk of the underlying pool.
