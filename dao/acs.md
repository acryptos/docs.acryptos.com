# Tokenomics & Fees

## <mark style="color:red;">$ACS</mark> Token

### Liquidity

* Uniswap V3 (BSC): [Trade](https://app.1inch.io/#/56/advanced/swap/BNB/0x8888888888f004100C0353d657BE6300587A6CcD) / [Liquidity](https://app.uniswap.org/add/0x8888888888f004100C0353d657BE6300587A6CcD/ETH/10000?chain=bnb) Info: [US](https://app.uniswap.org/explore/pools/bnb/0x86D708404d0DB1D97843E66D4Ed6B86d11bE705B) / [DS](https://dexscreener.com/bsc/0x86D708404d0DB1D97843E66D4Ed6B86d11bE705B)
* Equilibre (Kava): [Trade](https://equilibrefinance.com/swap) / [Liquidity](https://app.acryptos.com/vaults/2222/0x05Aa420a97449c0C54B369BAfaA9Ca43a77004eD/) Info: [DS](https://dexscreener.com/kava/0x395e6e5f3df5120fda26be1849d4388cc2500435)

[Dex Screener Watchlist](https://dexscreener.com/watchlist/9qDR83Yk0EjRCCPE26sH)

### Bridge & Migration

* **Bridge ACS:** [https://app.acryptos.com/acs/bridge/](https://app.acryptos.com/acs/bridge/)\
  $ACS is native on BNB Chain. It can be used in a number of other chains through our bridge, developed via LayerZero.
* **Migrate ACS:** [https://app.acryptos.com/acs/migrate/](https://app.acryptos.com/acs/migrate/)\
  $ACS has been updated to a new token contract. This is due to a Multichain issue in 2023. Please migrate any of your original $ACS to the new contract. See below for full details.

### Tokenomics

$ACS emissions was initially supply capped at 1,888,888 tokens. Tokenomics was upgraded in July 2023 to cut off all emissions.&#x20;

{% hint style="info" %}
Current total supply can be tracked on [Coinmarketcap](https://coinmarketcap.com/currencies/acryptos/).
{% endhint %}

Fees collected from all ACryptoS vaults go to ACryptoS [Treasury](https://debank.com/profile/0x5bd97307a40dfbfdbaef4b3d997adb816f2dadcc) with periodical Buyback and Burning of the ACS token. Adding to the fact that there are no longer any ACS emissions, this results in a deflationary model for the $ACS token, benefiting ACS holders in the long term.

There is no $ACS vault staking. Users only need to hold the token in their wallet to receive the benefits from Buyback and Burn.

For users looking to pair $ACS into a liquidity pool for earning swap fees or token farming, existing pools can be found in the [Liquidity](acs.md#liquidity) section above.

_\*All parameters may be adjusted in future via governance._

<details>

<summary><strong>Multichain.org Incident - July 2023</strong></summary>

The Multichain.org bridge stopped working on 7 July 2023 following abnormal movements of locked assets. \~170K of bridged ACS was stuck and under the control of unknown entities. An announcement was made to ask users to remove ACS paired liquidity as a migration plan was being worked on. A governance vote was taken to [approve the migration](https://vote.acryptos.com/#/proposal/0x16b1bcf3b151f9de38b151616f5d83bfdc2415a677cd5953ec1be2d0343009e1).

A new ACS token is deployed at 0x8888888888f004100C0353d657BE6300587A6CcD across several chains.

The new token was designed with certain features to mitigate bridging risks:

* Bridging is achieved by passing cross chain messages. This is using Layer Zero initially, and can be upgraded to use any combination of protocols.
* ACryptoS Dev team controls new token contracts including the ability to pause and blacklist in the event of bridge / messaging protocol exploit.
* Bridged balances are reconciled on the canonical chain (BSC). Bridging can only be done to/from the canonical chain, and will fail if they cannot be reconciled (i.e. more balance bridged in than has been bridged out).

There is a [migration](acs.md#bridge-and-migration) feature which will allow users to migrate 1:1 the old/Multichain.org ACS tokens. Migration will be paused if the contract detects abnormal changes in the locked Multichain.org ACS tokens.

Withdraw from ACS vault with no penalty fees: [https://app-legacy.acryptos.com/core/](https://app-legacy.acryptos.com/core/)

</details>

<details>

<summary><mark style="color:red;">$ACS</mark> and <mark style="color:orange;">$ACSI</mark> Token Merger</summary>

There were discussions on simplifying ACryptoS tokenomics to a single token, and a [governance vote was passed](https://vote.acryptos.com/#/proposal/0xe9b6e77cfeafaf95556ed7e7d882d2792c0eaca32c317688f56cf7b037521de4) to merge $ACSI at a 4:1 ratio to the new $ACS token.

* Withdraw from $ACSI vault with no penalty fees: [https://app-legacy.acryptos.com/core/](https://app-legacy.acryptos.com/core/)
* $ACSI migration to $ACS token: [https://app.acryptos.com/acs/migrate/](https://app.acryptos.com/acs/migrate/)

</details>

\*_$ACS and $ACSI Tokenomics was upgraded in 2023. Link to original tokenomics can be found_ [_here_](fees-legacy.md)_._

***

## Fees

### All Vaults

**Withdrawal fee: 0.1%**

* Calculated from the total withdrawal amount.
* Goes to ACryptoS Treasury with periodical Buyback and Burn.

**Performance fee:** 4.5% of gains harvested goes to ACryptoS Treasury with periodical Buyback and Burn.

**Strategist fee:** 4.5% of gains harvested goes go strategy creator.

**Harvester subsidy fee:** up to 0.3% of gains harvested paid to any wallet compounding the vaults。\
See further details under Vault [Advanced Functions](../products/vaults/single-token-vaults.md#advanced-functions).

{% hint style="success" %}
_The above **performance / strategist / harvester fees** are transparent to users and already accounted for in the displayed "Vault APY". We disclose them here for transparency._
{% endhint %}

### StableSwap (Legacy)

[Stableswap](https://app-legacy.acryptos.com/stableswap/) is currently a Public Goods protocol on BSC. All fees go to liquidity providers. Exchange fee: 0.01%

### Acsi.Finance (Legacy)

[Acsi.Finance](https://app.acsi.finance) is currently a Public Goods protocol on BSC. All fees go to liquidity providers. Exchange fee: Variable (displayed on UI)
