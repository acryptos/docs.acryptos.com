---
description: >-
  Built on Balancer V2, Acsi.Finance brings the first next-generation AMM
  protocol to Binance Smart Chain.
---

# Acsi.Finance

## Quick Start

* [Trading](https://docs.balancer.fi/getting-started/walkthroughs/trading)
* [Investing](https://docs.balancer.fi/getting-started/walkthroughs/invest)

## What is Balancer?

Balancer is an automated portfolio manager, liquidity provider, and price sensor.

Balancer turns the concept of an index fund on its head: instead of paying fees to portfolio managers to rebalance your portfolio, you collect fees from traders, who rebalance your portfolio by following arbitrage opportunities.

Balancer is based on an [N-dimensional invariant surface](https://balancer.finance/whitepaper/) which is a generalization of the constant product formula described by Vitalik Buterin and proven viable by the popular Uniswap dapp.

Balancer V2 brings powerful new features to slash gas costs, super-charge capital efficiency, unlock arbitrage with zero-token starting capital, and open the door to custom AMMs.

## Additional Resources

* [Balancer V2 documentation](https://docs.balancer.fi/)
* [Balancer V2 FAQs](https://docs.balancer.fi/getting-started/faqs)

## Security & Audits

Acsi.Finance uses Balancer V2 contracts verbatim, which have completed [several full audits](https://docs.balancer.fi/core-concepts/security/audits) and have a comprehensive [bug bounty](https://docs.balancer.fi/core-concepts/security/bug-bounties) program.

## Price Impact for Liquidity Providers

When you deposit into an Acsi.Finance pool, you receive an LP token representing a share of that pool. This represents all tokens in the pool at the proportions they are currently in.

If you deposit or withdraw in proportions which are different from the pool's current proportions, what happens behind the scenes is that the tokens are exchanged so it matches the proportions of the pool.

A pool is "balanced" when the value of its tokens matches their weights. For example, a BNB/ETH/BTC 33%/33%/33% pool is "balanced" when it has $1M worth of BNB, ETH and BTC _each_.

Any transaction - trade / deposit / withdrawal - that brings a pool into "balance" would result in a "profit" - i.e. you would be able to arbitrage it for a profit. And vice-versa - any transaction bringing a pool "off-balance" would result in a "loss" - someone would then be able to arbitrage the pool for a profit.



