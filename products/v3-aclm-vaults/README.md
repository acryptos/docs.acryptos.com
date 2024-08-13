# ACLM - Advanced Concentrated Liquidity Manager

Our ACLM is built on top of V3 Conc. Liquidity DEXs (namely UniswapV3 and its forks). Using uniquely developed strategies, we improve swap rate efficiency for liquidity pairs (less slippage), and we achieve a higher than average APY for users providing liquidity.

Key features of our ACLM include:

* Dynamic setting of positions and ranges.
* Automated rebalancing for optimal yields.
* Simplified single-token deposit system.

Our Strategy automatically compounds fees and rebalances its position around the current price. This streamlines the liquidity provision process, reducing additional actions from users, earning them sustainable yields via swap fees.

<details>

<summary>Understanding Conc. Liquidity - A Quick Look</summary>

How conc. liquidity works is by letting users be strategic about their liquidity provisioning. Instead of spreading your assets across the entire price range, you can choose a specific price zone to focus on. This allows you to earn higher fees on trades that happen within your chosen zone.

**Caveat:** While concentrated liquidity offers much higher APY when trades happen in your set range, it also comes with trade-offs. Once trades move outside your chosen price zone, there will be zero fees rewarded, and extreme price movements can lead to imbalanced positions and impermanent losses that are much higher than V2 LPs.

A detailed understanding of V3 Concentrated Liquidity can be found [here](https://docs.uniswap.org/concepts/protocol/concentrated-liquidity) in Uniswap docs.

</details>

## How our ACLM stands out

Our ACLM distinguishes itself from other liquidity managers by maintaining a dynamic range on V3 positions, adjusting to be narrower or wider depending on price fluctuation and volatility trends. This approach ensures that we consistently manage to host active liquidity, leading to more efficient swap volumes.

**Examples of past performance:**

* Stable vaults delivering consistently strong yields over a number of months, eg.
  * USDC/DAI at 20-30+% APY
  * wstETH/ETH at 10+% APY
  * WBTC/BTC.b at 10+% APY
* High-yield returns on volatile pairs, successfully countering impermanent losses, eg.
  * ARB/ETH at 101+% APY
  * BTC/ETH at 36+% APY \*_the above APY are all achieved purely via swap fees_
* Dominating over 90% of active liquidity in OP Chain's USDT/DAI and USDC/USDT pools ([link](https://app.acryptos.com/u3i/pools/10/0xF1F199342687A7d78bCC16fce79fa2665EF870E1/?a=0x9F0d1DB674488eaF2DE5fd722176CD751803fEf5))
* Hosted 20%+ of active liquidity in OP Chain's wstETH/ETH pools
* Hosted 50%+ of active liquidity in Base Chain's USDC/USDbC pool

![Screenshot of managed USDT-DAI (Optimism) active liquidity %](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/u3i%20-%20Optimism%20USDT-DAI.jpg)

\*_managing 88.3% of active trading liquidity for USDT/DAI Uniswap V3 (Optimism) - 28 Feb '24_

Find out more about our Strategies here:

{% content-ref url="strategies.md" %}
[strategies.md](strategies.md)
{% endcontent-ref %}

## Understanding the Source of APY

Many defi users that have been depositing in V2 LPs may be familiar with the farming mechanism, where staking an LP gets you APY from DEX farming tokens. APY from V3 Conc. Liquidity pools comes mainly from swap fees, providing a sustainable source of yield for liquidity providers.

Some additional APY are added as incentives via Merkl. Our vaults are designed to harvest the rewards and compound them for users automatically.

## Exploit Risk Mitigations

The multi-token nature of the vaults and their auto-rebalancing feature on concentrated liquidity AMMs make them vulnerable to price manipulation/flash loan type attacks. We have implemented some mitigations to address this:

* We use historical TWAP to detect price volatility / manipulation, which pauses Vault functionality.
* There is a cooldown period after every vault rebalance, which pauses Vault functionality.
* Deposits and withdrawals are subject to slippage checks. Users should check and confirm the correct amounts to be received on the UI before signing transactions.

The risk of attacks increases as Vault TVL forms the bulk of the underlying pool.
