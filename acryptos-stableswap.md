---
description: >-
  ACryptoS StableSwap is an automated market maker (AMM) enabling fast and
  efficient stablecoin trading at the best prices with low slippage and fees on
  Binance Smart Chain.
---

# ACryptoS StableSwap

## Cheaper Better Faster

ACryptoS StableSwap offers
 - ~10X lower exchange fee
 - ~500X smaller slippage

as compared to various UniSwap type AMMs on Binance Smart Chain. 

This is due to the usage of Curve's [specialized algorithm tailored for trading of stablecoins and other pegged assets](https://www.curve.fi/stableswap-paper.pdf).

Trading on Binance Smart Chain also means gas costs up to **~100X cheaper** than on Ethereum, and a **~5X faster** block interval of 3 seconds.

## Yield Farming with ACSI <a id="b267"></a>

We share a stake in the protocol with ACryptoS StableSwap liquidity providers, distributing ACSI tokens via our farms. 50% of exchange fees are used to buy back and distribute ACSI to ACSI stakers via the ACSI Vault, while the remainder are earned by liquidity providers.

Do remember to stake in our Farms after depositing into the pools.

## ACS4USD Corepool

Our core pool comprises the 4 staple stablecoins: BUSD, USDT, DAI and USDC.

## ACS4 + VAI / UST / QUSD Metapools

These metapools allow seamless trading between the metapool's additional token, and all 4 tokens in the ACS4USD core-pool.

Metapools allow for one token to seemingly trade with another underlying base pool with several benefits:

* Prevents dilution of base pool.
* Allows listing of less liquid assets.
* Base pool holders are shielded from systemic risks of the metapool. \(i.e. should VAI lose it's peg, ACS4USD corepool liquidity providers who did not provide liquidity to the metapool will not be affected\)

## Price Impact for Liquidity Providers

When you deposit into a StableSwap pool or metapool, you receive an LP token representing a share of that pool. This represents all tokens in the pool at the proportions they are currently in. These proportions change whenever there is a swap, but in the long run, as long as the tokens maintain their peg, the proportions should revert equally.

If you deposit or withdraw in proportions which are different from the pool's current proportions, what happens behind the scenes is that the tokens are exchanged so it matches the proportions of the pool. This effectively means if you deposit a token that the pool has a lower proportion of, you will get a "positive" price impact, and vice versa.

In general, if the token's market prices are at peg, it would be profitable to help "rebalance" the pool by depositing or withdrawing. However this might not be the case if prices are off peg. For example, if DAI's market price is significantly above peg, it's proportion in the pool should be much lower than the others'. If you deposit more DAI, you might see a "positive" price impact but depositing too much would push the price of DAI in the pool down and arbitrageurs would be able to buy it from the pool and sell it elsewhere for a profit.

Do note for metapools, a balanced proportion is achieved when the non-base token is equal to the base pool. For example, when ACS4VAI has 50% VAI and 50% ACS4.

