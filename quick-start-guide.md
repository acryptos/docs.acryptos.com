---
description: Getting to know our UI and how to pick between vaults.
---

# Quick-Start Guide

<figure><img src="https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/Docs%20-%20UI%20main%20page.png" alt=""><figcaption><p>https://app.acryptos.com</p></figcaption></figure>

## Vault Comparisons

You see some great yields on our dapp: there's [Single-Token](products/vaults/) vaults, and [ACLM](products/v3-aclm-vaults/) vaults - but you're not too sure which to pick. What are the _risks involved_? What tokens do you _receive as APY_? etc.

**This will help you out.** 👇

<table><thead><tr><th width="117"></th><th width="188">Single-Token Vaults</th><th>ACLM - Stable Strategies</th><th>ACLM - Volatile Strategies</th></tr></thead><tbody><tr><td>Built On</td><td><mark style="color:blue;">lending protocols, eg. Venus, Moonwell</mark></td><td><mark style="color:orange;">CL DEXs, eg. UniswapV3, SushiV3</mark></td><td><mark style="color:orange;">CL DEXs, eg. UniswapV3, SushiV3</mark></td></tr><tr><td>APY Source</td><td><mark style="color:blue;">supply/borrow APY</mark><br><mark style="color:blue;">+ lending platform tokens</mark></td><td><mark style="color:orange;">swap fees generated from trading volume</mark><br><mark style="color:orange;">+ *</mark><a data-footnote-ref href="#user-content-fn-1"><mark style="color:orange;">Merkl rewards</mark></a></td><td><mark style="color:orange;">swap fees generated from trading volume</mark><br><mark style="color:orange;">+ *</mark><a data-footnote-ref href="#user-content-fn-2"><mark style="color:orange;">Merkl rewards</mark></a></td></tr><tr><td>Strategy Features</td><td><mark style="color:blue;">self-balancing for optimized highest APY</mark></td><td><ul><li><mark style="color:orange;">single-sided deposits of either token.</mark></li><li><mark style="color:orange;">auto range setting to ensure earning of swap fees</mark></li><li><mark style="color:yellow;">Tightened range for highest stable pair APY</mark></li></ul></td><td><ul><li><mark style="color:orange;">single-sided deposits of either token.</mark></li><li><mark style="color:orange;">auto range setting to ensure earning of swap fees</mark></li></ul></td></tr><tr><td>Examples</td><td><ul><li><mark style="color:blue;">USDT</mark></li><li><mark style="color:blue;">wstETH</mark></li><li><mark style="color:blue;">BTC</mark></li><li><mark style="color:blue;">LINK</mark></li></ul></td><td><ul><li><mark style="color:orange;">USDC-DAI</mark></li><li><mark style="color:orange;">USDC-USDC.e</mark></li><li><mark style="color:orange;">wstETH-WETH</mark></li><li><mark style="color:orange;">cbETH-rETH</mark></li><li><mark style="color:orange;">WBTC-tBTC</mark></li></ul></td><td><ul><li><mark style="color:orange;">MATIC-USDT</mark></li><li><mark style="color:orange;">LINK-WETH</mark></li><li><mark style="color:orange;">BTC-WETH</mark></li><li><mark style="color:orange;">USDC-XSGD</mark></li></ul></td></tr></tbody></table>

**More detailed comparisons here:**

|                                     | Single-Token Vaults                                                                                                                                                                                                                                               | ACLM - Stable Strategies                                                                                                                                                                                                                 | ACLM - Volatile Strategies                                                                                                                                                                                                                    |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Risks](quick-start-guide.md#risks) | <ul><li><mark style="color:blue;">lending protocol exploits</mark></li><li><mark style="color:yellow;">no IL risks</mark></li></ul>                                                                                                                               | <ul><li><mark style="color:orange;">CL DEX exploits</mark></li><li><mark style="color:yellow;">low chances of IL</mark></li></ul>                                                                                                        | <ul><li><mark style="color:orange;">CL DEX exploits</mark></li><li><mark style="color:yellow;">high IL risks</mark></li></ul>                                                                                                                 |
| Considerations                      | <ul><li><mark style="color:blue;">exposure to 1 token</mark></li><li><mark style="color:blue;">slower growth of tokens</mark></li><li><mark style="color:blue;">high APY vaults less sustainable (as mainly coming from lending platform tokens)</mark></li></ul> | <ul><li><mark style="color:orange;">exposure to 2 tokens</mark></li><li><mark style="color:yellow;">higher APY, for relatively low IL risk</mark></li><li><mark style="color:orange;">rewards sustainable via swap fees</mark></li></ul> | <ul><li><mark style="color:orange;">exposure to 2 tokens</mark></li><li><mark style="color:yellow;">highest APY, but gains easily negated by IL</mark></li><li><mark style="color:orange;">rewards sustainable via swap fees</mark></li></ul> |
| Rewards                             | <mark style="color:blue;">auto-compounding into deposited tokens</mark>                                                                                                                                                                                           | <mark style="color:blue;">auto-compounding into deposited tokens</mark>                                                                                                                                                                  | <mark style="color:blue;">auto-compounding into deposited tokens</mark>                                                                                                                                                                       |
| Links                               | [https://app.acryptos.com/vaults/single/](https://app.acryptos.com/vaults/single/)                                                                                                                                                                                | [https://app.acryptos.com/aclm/](https://app.acryptos.com/aclm/)                                                                                                                                                                         | [https://app.acryptos.com/aclm/](https://app.acryptos.com/aclm/)                                                                                                                                                                              |

{% hint style="info" %}
Notes:

* IL: impermanent loss
* CL: [concentrated liquidity](https://docs.uniswap.org/concepts/protocol/concentrated-liquidity)
* DEX: decentralized exchange
* LST: [liquid staking tokens](https://chain.link/education-hub/liquid-staking)
* LRT: [liquid restaking tokens](https://www.coindesk.com/learn/restaking-101-what-are-restaking-and-liquid-restaking/)
{% endhint %}

***

## Categories

<figure><img src="https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/Docs%20-%20UI%20categories.png" alt=""><figcaption></figcaption></figure>

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

***

**Examples:**

**Single-Token Vaults**

* USDC on Venus (BSC)
* USDC.e on Lodestar (Arbitrum)
* USDbC on Moonwell (Base)
* xcUSDC on Moonwell (Moonbeam)

**ACLM - Stable Strategies**

* USDC.e / axlUSDC on UniswapV3 (Polygon)
* USDC.e / USDC on UniswapV3 (Optimism)
* USDbC / axlUSDC on SushiswapV3 (Base)

Link: [https://app.acryptos.com/vaults/?a=usd-a](https://app.acryptos.com/vaults/?a=usd-a)
{% endtab %}

{% tab title="USD-B" %}
A category of stablecoins from various protocols, ranging from large marketcap to algorithm pegged USD stable tokens. Stablecoin pools paired with USDC also fall under this category.

* USDT (USD by [Tether](https://tether.to/en/))
  * centralized stablecoin pegged to the US dollar
  * largest marketcap among stablecoins
* DAI by [MakerDAO](https://makerdao.com/en/)
  * largest decentralized stablecoin pegged to the US dollar
  * algorithmically backed by a basket of cryptocurrencies, primarily ETH
* [Ethena USDe](https://ethena-labs.gitbook.io/ethena-labs/solution-overview/usde-overview)
* [Binance BUSD](https://www.coingecko.com/en/coins/binance-peg-busd)
* [Liquity LUSD](https://www.liquity.org/)
* [Verified USDV](https://usdv.money/)
* USDC.e (bridged USDC on chains [before USDC was natively available](https://www.datawallet.com/crypto/usdc-e-vs-usdc-explained))
* axlUSDC (bridged USDC by [Axelar](https://www.axelar.network/))
* USDbC (bridged USDC by [Base chain](https://help.coinbase.com/en/coinbase/getting-started/crypto-education/usd-base-coin))
* xcUSDC (XCM protocol USDC on [Polkadot parachains](https://help.circle.com/s/article/A-closer-look-at-Polkadot-USDC-and-the-XCM-protocol?language=en\_US))
* xcUSDT (XCM protocol USDT on Polkadot parachains)
* [FRAX](https://frax.finance/)
* S\*USDt by [Stargate](https://stargate.finance/pool) on [Kava EVM](https://www.kava.io/)

***

**Examples:**

* DAI on Venus (BSC)
* USDT on Moonwell (Optimism)
* USDT on Mendi (Linea)
* xcUSDT on Moonwell (Moonbeam)
* FRAX on Lodestar (Arbitrum)

**ACLM - Stable Strategies**

* USDC.e / DAI on UniswapV3 (Optimism)
* USDT / BUSD on PancakeswapV3 (BSC)
* USDT / USDC on UniswapV3 (Linea)
* DAI / USDbC on SushiswapV3 (Base)

Link: [https://app.acryptos.com/vaults/?a=usd-b](https://app.acryptos.com/vaults/?a=usd-b)
{% endtab %}

{% tab title="BTC" %}
A category of various types of wrapped and liquid staked BTC.

* WBTC - centralized and largest marketcap [wrapped BTC by BitGo](https://decrypt.co/resources/what-is-wbtc-explained-bitcoin-ethereum-defi)
* tBTC - decentralized wrapping [by Threshold Network](https://threshold.network/)
* BTCB - centralized and pegged [by Binance](https://www.bnbchain.org/en/blog/btcb-on-binance-smart-chain-101)
* BTC.b - decentralized wrapping [by Avalanche Network](https://support.avax.network/en/articles/6349640-how-does-the-avalanche-bridge-work)
* uniBTC - [liquid restaking WBTC](https://docs.bedrock.technology/multi-asset-liquid-staking/unibtc) by Bedrock
* cbBTC - [coinbase wrapped BTC](https://www.coinbase.com/cbbtc)

***

**Examples:**

**Single-Token Vaults**

* WBTC on Moonwell (Optimism)
* WBTC on Mendi (Linea)
* BTCB on Venus (BSC)
* cbBTC on Moonwell (Base)

**ACLM - Stable Strategies**

* WBTC / BTC.b on UniswapV3 (Arbitrum)
* WBTC / uniBTC on UniswapV3 (Optimism)
* WBTC / tBTC on SushiswapV3 (Arbitrum)

Link: [https://app.acryptos.com/vaults/?a=btc](https://app.acryptos.com/vaults/?a=btc)
{% endtab %}

{% tab title="ETH" %}
A category of various types of wrapped and liquid staked ETH.

* WETH - wrapped ETH on non Ethereum chains
* wstETH - liquid staking ETH [by Lido](https://help.lido.fi/en/articles/5231836-what-is-lido-s-wsteth)
* rETH - liquid staking ETH [by RocketPool](https://rocketpool.net/)
* cbETH - liquid staking ETH [by Coinbase](https://www.coinbase.com/cbeth)
* weETH - liquid staking ETH [by Ether.fi](https://etherfi.gitbook.io/etherfi/getting-started/faq)
* wBETH - liquid staking ETH [by Binance](https://www.binance.com/en/support/faq/what-is-wbeth-e252366155174ba6887f6b32e3798273)
* ezETH - liquid restaking ETH [by Renzo](https://www.renzoprotocol.com/)

***

**Examples:**

**Single-Token Vaults**

* WETH on Mendi (Linea)
* wstETH on Lodestar (Arbitrum)
* cbETH on Moonwell (Base)
* rETH on Moonwell (Optimism)

**ACLM - Stable Strategies**

* wstETH / WETH on UniswapV3 (Optimism)
* cbETH / WETH on SushiswapV3 (Base)
* ETH / wBETH on BiswapV3 (BSC)

Find out more on why our Stable Strategies [work so well](products/v3-aclm-vaults/strategies.md#stable-strategies) for LST vaults.

Link: [https://app.acryptos.com/vaults/?a=eth](https://app.acryptos.com/vaults/?a=eth)
{% endtab %}

{% tab title="ETH+" %}
An ACLM category where liquid staked ETH from different platforms are paired together in a pool.

***

**Examples:**

**ACLM - Stable Strategies**

* wstETH / ezETH on UniswapV3 (Optimism)
* cbETH / rETH on UniswapV3 (Base)
* wstETH / rETH on UniswapV3 (Arbitrum)

Find out more on why our Stable Strategies [work so well](products/v3-aclm-vaults/strategies.md#stable-strategies) for LST vaults.

Link: [https://app.acryptos.com/vaults/?a=eth%2B](https://app.acryptos.com/vaults/?a=eth%2B)
{% endtab %}

{% tab title="BNB" %}
A category of various types of wrapped and liquid staked BNB.

* WBNB - wrapped BNB by Binance
* ankrBNB - liquid staking BNB [by Ankr](https://www.ankr.com/docs/liquid-staking/bnb/overview/)
* BNBx - liquid staking BNB [by Stader](https://www.staderlabs.com/blog/bnbx/)
* stkBNB - liquid staking BNB [by pSTAKE](https://blog.pstake.finance/stkbnb-faqs/)
* slisBNB - liquid staking BNB [by Lista](https://docs.bsc.lista.org/get-started/about-slisbnb) (previously Synclub staked SnBNB)

***

**Examples:**

**Single-Token Vaults**

* WBNB on Venus (BSC)

**ACLM - Stable Strategies**

* WBTC / ankrBNB on PancakeswapV3 (BSC)
* WBTC / BNBx on PancakeswapV3 (BSC)
* WBTC / stkBNB on PancakeswapV3 (BSC)

Link: [https://app.acryptos.com/vaults/?a=bnb](https://app.acryptos.com/vaults/?a=bnb)
{% endtab %}

{% tab title="LP-A" %}
A category of ACLM vaults, consisting of large marketcap token pairs.

* WMATIC
* WETH
* WBNB
* WBTC
* tBTC
* BTCB
* BTC.b
* OP
* ARB

IL is relatively lower than other pairs as prices for large marketcap tokens generally move in the same direction.

_\*Take note that IL may negate any gains, or result in losses on the intial deposit. Refer to the_ [_History Graph_](products/v3-aclm-vaults/advanced-functions.md#graph-history) _in the Advanced section of each vault to evaluate their past performance._

***

**Examples:**

**ACLM - Volatile Strategies**

* BTCB / WBNB on PancakeswapV3 (BSC)
* WETH / ARB on SushiswapV3 (Arbitrum)
* WETH / OP on UniswapV3 (Optimism)
* WMATIC / WBTC on UniswapV3 (Polygon)
* tBTC / WETH on UniswapV3 (Arbitrum)

Link: [https://app.acryptos.com/vaults/?a=lp-a](https://app.acryptos.com/vaults/?a=lp-a)
{% endtab %}

{% tab title="LP-B" %}
A category of ACLM vaults, consisting of smaller marketcap tokens paired with large marketcap tokens.

_\*Liquidity for our ACryptoS_ [_governance token pair_](dao/acs.md) _ACS / WBNB can be found in this category as well._

Some of the tokens available:

* BSW, LODE, VELA, THALES, GMX, XVS, PEPE, CAKE, MAGIC, TIA.n, CRV, UNI, LINK

IL may be higher for these pairs as prices tend to fluctuate much more for lower marketcap tokens.

_\*Take note that IL may negate any gains, or result in losses on the intial deposit. Refer to the_ [_History Graph_](products/v3-aclm-vaults/advanced-functions.md#graph-history) _in the Advanced section of each vault to evaluate their past performance._

***

**Examples:**

**ACLM - Volatile Strategies**

* CAKE / WBNB on PancakeswapV3 (BSC)
* LINK / WETH on UniswapV3 (Arbitrum)
* PEPE / WETH on UniswapV3 (Arbitrum)
* CRV / WETH on UniswapV3 (Arbitrum)
* UNI / WETH on UniswapV3 (Arbitrum)
* BSW / WBNB on BiswapV3 (BSC)

Link: [https://app.acryptos.com/vaults/?a=lp-b](https://app.acryptos.com/vaults/?a=lp-b)
{% endtab %}

{% tab title="LP-C" %}
A category of ACLM vaults, consisting of stablecoin tokens paired with mainly large marketcap tokens.

IL may be **very high** for these pairs as fluctuating token prices are amplified when paired with stablecoin tokens.

_\*Take note that IL may negate any gains, or result in losses on the intial deposit. Refer to the_ [_History Graph_](products/v3-aclm-vaults/advanced-functions.md#graph-history) _in the Advanced section of each vault to evaluate their past performance._

***

**Examples:**

**ACLM - Volatile Strategies**

* WBNB / USDT on UniswapV3 (BSC)
* wstETH / USDC.e on UniswapV3 (Arbitrum)
* MATIC / USDT on UniswapV3 (Polygon)
* WETH / USDbC on UniswapV3 (Base)
* WETH / USDC on SushiswapV3 (Arbitrum)

Link: [https://app.acryptos.com/vaults/?s=tvl\&a=lp-c](https://app.acryptos.com/vaults/?s=tvl\&a=lp-c)
{% endtab %}

{% tab title="LP-FIAT" %}
A category of stablecoins from different currencies, paired with the USD stablecoin.

IL is minimal, as pegged fiat currencies are much less volatile than other crypto tokens. Token unpeg risk has to be factored in as part of risk assessment as well.

* XSGD [by StraitsX](https://www.straitsx.com/xsgd)
* EURC [by Circle](https://www.circle.com/en/eurc)

**ACLM - Volatile Strategies**

* XSGD / USDC.e on UniswapV3 (Polygon)
* XSGD / USDC on UniswapV3 (Arbitrum)
* EURC / USDC on UniswapV3 (Base)

Link: [https://app.acryptos.com/vaults/?s=tvl\&a=lp-fiat](https://app.acryptos.com/vaults/?s=tvl\&a=lp-fiat)
{% endtab %}
{% endtabs %}

***

## Risks

DeFi risks are very high compared to traditional finance, ranging widely from market factors to contract exploits. Here are some risks for consideration along with possible mitigations. Factor in your own risk appetite when deciding on which vaults to deposit your tokens in.

{% hint style="warning" %}
Only put in funds you can afford to lose. Do not risk your life savings on DeFi.
{% endhint %}

<details>

<summary>General Smart Contract Risks</summary>

Smart contracts are vulnerable to exploits. These exploits can result in significant financial losses or other negative consequences. It's crucial to understand the risks involved and avoid interacting with contracts from untrusted sources.

ACryptoS has focused on safety and careful risk assessment since deployment in 2020. Multiple [audits](dao/security-and-risks.md#audits) and a [bug bounty](dao/bug-bounty.md) serve to enhance the security. Read our blog here to understand [what sets us apart](https://medium.com/acryptos/what-sets-acryptos-apart-d6345e2f5d7f).

</details>

<details>

<summary>Vaults - Underlying Protocol Risks</summary>

* our Single-Token vaults are built on top of lending protocols. They run the risk where the underlying protocols are exploited, and funds siphoned out via exploiters. We aim to filter out projects via thorough internal due diligence procedures, and try our best to build on safe credible protocols. Over the years since our deployment, despite our best efforts, there have been a few of these protocols exploited with funds unrecoverable (read: [Atlantis](https://t.me/acryptos/1/230896), [Channels](https://t.me/acryptos/1/238945), [Sonne](https://medium.com/@SonneFinance/post-mortem-sonne-finance-exploit-12f3daa82b06))
* our ACLM vaults are built on top of V3 Conc Liquidity DEXs. In order to minimize the risks of exploits on the underlying DEX, we aim to only build on stronger and battle-tested DEXs like Uniswap, Sushi, and Pancakeswap.

</details>

<details>

<summary>Stablecoin Depeg Risks</summary>

* protocols issuing USD stablecoins claim to be pegged to USD 1:1, but many smaller marketcap stablecoins are at a high risk of depegging. It may be due to the mechanics behind how the stablecoin is backed, or due to market sentiments resulting in sell-offs, etc.
* larger stablecoins like USDC, USDT, DAI, etc have lower depeg risks, though there have been multiple depegging issues over the years as well

</details>

<details>

<summary>LST/LRT Protocol Risks</summary>

* liquid staking tokens tend to be quite centralized, where user funds like ETH or BNB are held by the intermediary protocol, and staking is done on their back end.
* Risks involve protocol exploits, intentional draining of funds, or "depegging" of liquid staked tokens . Lack of liquidity might affect the unstaking of liquid tokens back to the native token as well.
* eg. rETH, wstETH, cbETH, stkBNB, ankrBNB, BNBx etc.
* please DYOR on how credible and transparent the staking protocols are, as well as how large the market of these tokens are

</details>

<details>

<summary>Bridged Token Risks</summary>

* it is essential to understand the difference between native tokens and bridged tokens on various chains. Bridged tokens are susceptible to risks and exploits of the bridging protocol itself.&#x20;
* eg. USDC.e is a bridged token while USDC is the native token that is issued directly by Circle. The native USDC token can be redeemed 1:1 to USD via Circle.
* eg. Multichain bridge was exploited on multiple chains in 2023. Funds that were lost due to that incident has not been recovered since.

</details>

<details>

<summary>Wrapped Token Risks</summary>

Wrapped tokens, while offering convenience, can pose risks. The underlying asset's security and the wrapping platform's reliability are crucial factors. Be cautious of potential vulnerabilities and always research before investing in wrapped tokens.

eg. WBTC is wrapped by BitGo, cbBTC is wrapped by Coinbase etc.&#x20;

</details>

Read more about risks and mitigations [here](dao/security-and-risks.md).

***

## Fees

* Withdrawal Fees: All vaults have a 0.1% withdrawal fee, calculated by the withdrawal amount.
* Performance Fees: already factored into the displayed APY. Full details can be found [here](dao/fees.md).

{% hint style="info" %}
Tips from the Samurai:

Based on the daily yield rate, try to withdraw only after withdrawal fee is covered. It will be all nett profits from thereon.
{% endhint %}

All fees go to ACryptoS Treasury, used for frequent [buybacks](https://t.me/acryptos/1/242722) of the $ACS token.

Treasury is owned by ACryptoS DAO ($ACS token holders), managed by a multisig.

* Treasury current holdings can be tracked on [debank](https://debank.com/profile/0x5BD97307A40DfBFDBAEf4B3d997ADB816F2dadCC).
* More info on Governance [here](dao/governance.md).

***

### Next Steps 🚀

Interested to gain yields via our vaults?\
Check out this [step-by-step visual guide](tutorials-guides/step-by-step-guide.md).

{% content-ref url="tutorials-guides/step-by-step-guide.md" %}
[step-by-step-guide.md](tutorials-guides/step-by-step-guide.md)
{% endcontent-ref %}

[^1]: additional tokens offered by other platforms as incentives for providing liquidity on a CL DEX. Usually only liquidity provided within the trading range will receive these rewards.

[^2]: additional tokens offered by other platforms as incentives for providing liquidity on a CL DEX. Usually only liquidity provided within the trading range will receive these rewards.
