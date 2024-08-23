---
description: Getting to know our UI and vaults.
---

# Quick-Start Guide

<figure><img src="https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/Docs%20-%20UI%20main%20page.png" alt=""><figcaption><p>https://app.acryptos.com</p></figcaption></figure>

## Vault Comparisons

You see some great yields on our dapp, but you're not too sure which to pick.\
What are the _risks involved_? What tokens do you _receive as APY_? etc.

**This will help you out.**

<table><thead><tr><th width="117"></th><th width="188">Single-Token Vaults</th><th>ACLM - Stable Strategies</th><th>ACLM - Volatile Strategies</th></tr></thead><tbody><tr><td>Built On</td><td>lending protocols, eg. Venus, Moonwell</td><td>CL DEXs, eg. UniswapV3, SushiV3</td><td>CL DEXs, eg. UniswapV3, SushiV3</td></tr><tr><td>APY Source</td><td>supply/borrow APY<br>+ lending platform tokens</td><td>swap fees generated from trading volume<br>+ *<a data-footnote-ref href="#user-content-fn-1">Merkl rewards</a></td><td>swap fees generated from trading volume<br>+ *<a data-footnote-ref href="#user-content-fn-2">Merkl rewards</a></td></tr><tr><td>Strategy Features</td><td>self-balancing for optimized highest APY</td><td><ul><li>single-sided deposits of either token.</li><li>auto range setting to ensure earning of swap fees</li><li>Tightened range for highest stable pair APY</li></ul></td><td><ul><li>single-sided deposits of either token.</li><li>auto range setting to ensure earning of swap fees</li></ul></td></tr><tr><td>Examples</td><td><ul><li>USDT</li><li>wstETH</li><li>BTC</li><li>LINK</li></ul></td><td><ul><li>USDC-DAI</li><li>USDC-USDC.e</li><li>wstETH-WETH</li><li>cbETH-rETH</li><li>WBTC-tBTC</li></ul></td><td><ul><li>MATIC-USDT</li><li>LINK-WETH</li><li>BTC-WETH</li><li>USDC-XSGD</li></ul></td></tr></tbody></table>

**More info:**

|                                     | Single-Token Vaults                                                                                                                                    | ACLM - Stable Strategies                                                                                                        | ACLM - Volatile Strategies                                                                                                           |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| [Risks](quick-start-guide.md#risks) | <ul><li>lending protocol exploits</li><li>no IL risks</li></ul>                                                                                        | <ul><li>CL DEX exploits</li><li>low chances of IL</li></ul>                                                                     | <ul><li>CL DEX exploits</li><li>high IL risks</li></ul>                                                                              |
| Considerations                      | <ul><li>exposure to 1 token</li><li>slower growth of tokens</li><li>rewards less sustainable (as mainly coming from lending platform tokens)</li></ul> | <ul><li>exposure to 2 tokens</li><li>higher APY, for relatively low IL risk</li><li>rewards sustainable via swap fees</li></ul> | <ul><li>exposure to 2 tokens</li><li>highest APY, but gains easily negated by IL</li><li>rewards sustainable via swap fees</li></ul> |
| Rewards                             | auto-compounding into deposited tokens                                                                                                                 | auto-compounding into deposited tokens                                                                                          | auto-compounding into deposited tokens                                                                                               |
| Links                               | [https://app.acryptos.com/vaults/single/](https://app.acryptos.com/vaults/single/)                                                                     | [https://app.acryptos.com/aclm/](https://app.acryptos.com/aclm/)                                                                | [https://app.acryptos.com/aclm/](https://app.acryptos.com/aclm/)                                                                     |

{% hint style="info" %}
Notes:

* IL: impermanent loss
* CL: concentrated liquidity
* DEX: decentralized exchange
* LST: liquid staking tokens
* LRT: liquid restaking tokens
{% endhint %}

## Categories

{% tabs %}
{% tab title="USD-A" %}
A category of higher quality stablecoins vaults, built on USDC and its bridged counterparts.

* USDC (USD Coin by [Circle](https://www.circle.com/en/usdc))
  * see [here](https://www.circle.com/en/multi-chain-usdc) for chains that USDC is native on
  * native USDC has 1:1 backing, transparent, verified reserves.
* USDC.e (bridged USDC on chains [before USDC was natively available](https://www.datawallet.com/crypto/usdc-e-vs-usdc-explained))
* axlUSDC (bridged USDC by [Axelar](https://www.axelar.network/))
* USDbC (bridged USDC by [Base chain](https://help.coinbase.com/en/coinbase/getting-started/crypto-education/usd-base-coin))
* xcUSDC (XCM protocol USDC on [Polkadot parachains](https://help.circle.com/s/article/A-closer-look-at-Polkadot-USDC-and-the-XCM-protocol?language=en\_US))

### Examples

#### Single-Token Vaults

* USDC on Venus (BSC)
* USDC.e on Lodestar (Arbitrum)
* USDbC on Moonwell (Base)
* xcUSDC on Moonwell (Moonbeam)

#### ACLM - Stable Strategies

* USDC.e / axlUSDC on UniswapV3 (Polygon)
* USDC.e / USDC on UniswapV3 (Optimism)
* USDbC / axlUSDC on SushiswapV3 (Base)
{% endtab %}

{% tab title="USD-B" %}
A category of stablecoins from various protocols, ranging from large marketcap to algorithm pegged USD stable tokens. Various stables paired with USDC also fall under this category.

* USDT (USD by [Tether](https://tether.to/en/))
  * centralized stablecoin pegged to the US dollar
  * largest marketcap among stablecoins
* DAI by [MakerDAO](https://makerdao.com/en/)
  * largest decentralized stablecoin pegged to the US dollar
  * algorithmically backed by a basket of cryptocurrencies, primarily ETH
* USDe
* BUSD
* LUSD
* USDV
* USDC.e (bridged USDC on chains [before USDC was natively available](https://www.datawallet.com/crypto/usdc-e-vs-usdc-explained))
* axlUSDC (bridged USDC by [Axelar](https://www.axelar.network/))
* USDbC (bridged USDC by [Base chain](https://help.coinbase.com/en/coinbase/getting-started/crypto-education/usd-base-coin))
* xcUSDC (XCM protocol USDC on [Polkadot parachains](https://help.circle.com/s/article/A-closer-look-at-Polkadot-USDC-and-the-XCM-protocol?language=en\_US))

### Examples


{% endtab %}

{% tab title="LP-A" %}

{% endtab %}

{% tab title="LP-B" %}

{% endtab %}

{% tab title="LP-C" %}

{% endtab %}

{% tab title="LP-FIAT" %}

{% endtab %}

{% tab title="ETH+" %}

{% endtab %}
{% endtabs %}

## Risks

DeFi risks are very high compared to traditional finance, ranging widely from market factors to contract exploits. Here are some risks for consideration along with possible mitigations. Factor in your own risk appetite when deciding on which vaults to deposit your tokens in.

{% hint style="warning" %}
Only put in funds you can afford to lose. Do not risk your life savings on DeFi.
{% endhint %}

<details>

<summary>Protocol smart contract risks</summary>

ACryptoS has focused on safety and careful risk assessment since deployment in 2020. Multiple audits and a bug bounty serve to enhance the security. Read our blog here to understand [what sets us apart](https://medium.com/acryptos/what-sets-acryptos-apart-d6345e2f5d7f).

</details>

<details>

<summary>Vault underlying protocol risks</summary>

* our Single-Token vaults are built on top of lending protocols. They run the risk where funds are siphoned out via exploiters. We filter out projects via internal due diligence procedures, and try our best to build on safe credible protocols. Unfortunately, a few of these protocols were exploited and funds unrecoverable (read: Atlantis, Channels, Sonne)
* our ACLM vaults are built on top of V3 Conc Liquidity DEXs. We only build on stronger and battle-tested DEXs like Uniswap, Sushi, and Pancakeswap.

</details>

<details>

<summary>Stablecoin depeg risks</summary>

* many USD stablecoins claim to be pegged to USD 1:1, but many smaller marketcap stablecoins are at a high risk of depegging
* larger stablecoins like USDC, USDT, DAI, etc have encountered depegging as well

</details>

<details>

<summary>LST/LRT protocol risks</summary>

* liquid staking tokens tend to be quite centralized, where user funds like ETH or BNB are held by their protocol, and staking is done on their back end.
* Risks involve protocol exploits, intentional draining of funds, or "depegging" of liquid staked tokens . Lack of liquidity might affect the unstaking of liquid tokens back to the native token as well.
* eg. rETH, wstETH, cbETH, stkBNB, ankrBNB, BNBx etc.
* DYOR on how credible and transparent the staking protocols are, as well as how large the market of these tokens are

</details>

<details>

<summary>bridged token risks</summary>

* understand the difference between native tokens and bridged tokens. Bridged tokens may involve native bridges and third-party bridges
* eg. USDC.e is a bridged token while USDC is the native token that is issued directly by Circle
* eg. multichain bridge was exploited on multiple chains in 2023. Funds that were lost due to that incident has not been recovered since.

</details>

<details>

<summary>wrapped token risks</summary>

eg. WBTC depegging risks

</details>

Read more about risks and mitigations [here](dao/security-and-risks.md).

## Fees&#x20;

All vaults have a 0.1% withdrawal fee, calculated by the withdrawal amount.

{% hint style="info" %}
Tips from the Samurai:

Based on the daily yield rate, try to withdraw only after withdrawal fee is covered. It will be all nett profits from thereon.
{% endhint %}

Performance fees on vaults are already factored into the APY. Details can be found [here](dao/fees.md).

All fees go to ACryptoS Treasury, with frequent [buybacks](community.md) of the $ACS token.

Treasury is owned by ACryptoS DAO ($ACS token holders), managed by a multi-sig. More info on Governance [here](dao/governance.md).

[^1]: additional tokens offered by other platforms as incentives for providing liquidity on a CL DEX. Usually only liquidity provided within the trading range will receive these rewards.

[^2]: additional tokens offered by other platforms as incentives for providing liquidity on a CL DEX. Usually only liquidity provided within the trading range will receive these rewards.
