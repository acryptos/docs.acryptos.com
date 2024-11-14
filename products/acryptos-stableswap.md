---
description: >-
  ACryptoS StableSwap is an automated market maker (AMM) enabling fast and
  efficient stablecoin trading at the best prices with low slippage and fees on
  Binance Smart Chain.
---

# DEX - ACSI StableSwap

## Cheaper Better Faster

ACryptoS StableSwap is an [automated market maker (AMM)](https://academy.binance.com/en/articles/what-is-an-automated-market-maker-amm) protocol based on Curve’s specialized algorithm tailored for stable coins. ACryptoS is offering the first AMM for stable coins based on this algorithm on the Binance Smart Chain (BSC).

Trading on the Binance Smart Chain is both faster and significantly cheaper than trading on the Ethereum chain. ERC-20 Tokens can be crossed over from Ethereum to Binance Smart Chain via the Binance Bridge.

Acryptos StableSwap enables efficient stablecoin trading at best prices which is

* **\~10x lower exchange fee**;
* **\~100x less slippage** when trading stable coins compared to the various UniSwap type AMMs available.

as compared to various UniSwap type AMMs on Binance Smart Chain.

This is due to the usage of Curve's [specialized algorithm tailored for trading of stablecoins and other pegged assets](https://www.curve.fi/stableswap-paper.pdf).

Trading on Binance Smart Chain also means gas costs up to **\~100X cheaper** than on Ethereum, and a **\~5X faster** block interval of 3 seconds.

Resources:

Find out more about [Stablecoins](https://academy.binance.com/en/articles/what-are-stablecoins).

Find out more about [AMM and Liquidity Provider](https://academy.binance.com/en/articles/what-is-an-automated-market-maker-amm).

[How to use ACryptoS StableSwap (Video Tutorial)](https://www.youtube.com/watch?v=xn-apvGCsFY) - contributed by [CryptoBKT (Hsing)](https://t.me/cryptoBKT)

[Frequently Asked Questions](../faq.md)

## Yield Farming with ACSI <a href="#b267" id="b267"></a>

We share a stake in the protocol with ACryptoS StableSwap liquidity providers, distributing ACSI tokens via our farms.

50% of exchange fees are used to buy back and distribute ACSI to ACSI stakers via the ACSI Vault, while the remainder 50% are earned by liquidity providers.

Do remember to stake in our Farms after depositing into the pools.

## ACS4USD Corepool

Our core pool comprises the four stablecoins: 1. BUSD 2. USDT 3. DAI 4. USDC

## ACS4 + VAI / UST / QUSD Metapools

These metapools allow seamless trading between the metapool's additional token, and all 4 tokens in the ACS4USD core-pool.

Metapools allow for one token to seemingly trade with another underlying base pool with several benefits:

1.Prevents dilution of base pool.

2.Allows listing of less liquid assets.

3.Base pool holders are shielded from systemic risks of the metapool. (i.e. should VAI lose it's peg, ACS4USD corepool liquidity providers who did not provide liquidity to the metapool will not be affected)

## Price Impact for Liquidity Providers

When you deposit into a StableSwap pool or metapool, you receive an LP token representing a share of that pool. This represents all tokens in the pool at the proportions they are currently in.

These proportions change whenever there is a swap, but in the long run, as long as the tokens maintain their peg, the proportions should revert equally.

If you deposit or withdraw in proportions which are different from the pool's current proportions, what happens behind the scenes is that the tokens are exchanged so it matches the proportions of the pool.

This effectively means if you deposit a token that the pool has a lower proportion of, you will get a "positive" price impact, and vice versa.

In general, if the token's market prices are at peg, it would be profitable to help "rebalance" the pool by depositing or withdrawing. However this might not be the case if prices are off peg. For example, if DAI's market price is significantly above peg, it's proportion in the pool should be much lower than the others'. If you deposit more DAI, you might see a "positive" price impact but depositing too much would push the price of DAI in the pool down and arbitrageurs would be able to buy it from the pool and sell it elsewhere for a profit.

Do note for metapools, a balanced proportion is achieved when the non-base token is equal to the base pool, i.e. when ACS4VAI has 50% VAI and 50% ACS4.

***

## Risk: StableSwap assets losing their pegs

When investing in stableswap pools, you are exposed to each of the assets in the pool and risk (impermanent) loss of funds if one of the coins loses its peg.

**Mitigation:**

ACryptoS has split the StableSwap pools into a core pool and a number of metapools. The core pool is made up of BUSD, USDT, DAI and USDC.

The meta pools each contain one additional asset (e.g., VAI). The risk of an asset losing its peg in the meta pools is higher than the core pool (this is also compensated by a higher APY in the meta pools).
