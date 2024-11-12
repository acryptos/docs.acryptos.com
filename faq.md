---
description: Frequently-Asked Questions
---

# FAQ

<details>

<summary>Why use ACryptoS vaults? </summary>

**Why not just use the underlying Lending or DEX platforms?**

Our vaults are developed with complex strategies that automate and optimize yields for users. This not only **reduces time and stress** spent on monitoring DeFi positions, but also enables users to obtain APY which they **could not achieve in normal scenarios**.

Example I - our Single-Token vaults built on Moonwell lending platform: The Moonwell dapp does not allow users to supply and borrow the same token.

However, our vaults are able to implement this at the contract level, achieving higher yields while ensuring no liquidation risks _(due to same-token supplying/borrowing)_. Our vaults are also set to automatically optimize the leverage ratio based on the market APY. Read more [here](products/vaults/).

Example II - our ACLM vaults built on Uniswap V3 DEX: Setting positions and ranges on V3 Concentrated Liquidity require a high amount of time monitoring the prices and adjusting positions when out of swap range.

Our vaults utilize a number of tools to form our strategies, from Chainlink Price Feed monitoring, to automated ACryptoS Keepers, to ensure our managed liquidity is always within swap range. We are able to maintain an extremely narrow 1-tick liquidity range for certain pools, achieving higher APY than other automated CL managers. Read more [here](products/v3-aclm-vaults/#how-our-aclm-stands-out).

</details>

<details>

<summary>What are the risks involved?</summary>

ACryptoS vaults are battle-tested, launched since 2020 and without any contract exploits. _Risks mitigations and audits can be found_ [_here_](dao/security-and-risks.md)_._&#x20;

Over the years , a number of other similar yield optimizers have [lost user funds](https://medium.com/acryptos/how-were-acryptos-venus-vaults-unaffected-while-other-yield-optimizers-lost-tens-of-millions-in-27bf4258dfb2), or similar automated CL managers [got exploited](https://medium.com/gamma-strategies/post-mortem-remediation-plan-9a62f10d90f3) due to loopholes in developed contracts. We believe in developing vaults with safety always in mind, and cutting out any fancy, risky fluff.

Check out [this article](https://medium.com/acryptos/what-sets-acryptos-apart-d6345e2f5d7f) on our blog - written since a few years back, but still very much our core ethos.

</details>

<details>

<summary>What are the fees for using the vaults?</summary>

Straightforward 0.1% fee on withdrawal amount.

Other fees like performance or strategist fees are already factored into the APY. Find out more [here](dao/fees.md#fees).

</details>

<details>

<summary>Help, I can't find my deposits on the site!</summary>

Fret not, check these links first:\
\- [https://app.acryptos.com/vaults/deprecated/](https://app.acryptos.com/vaults/deprecated/)\
\- [https://app-legacy.acryptos.com/](https://app-legacy.acryptos.com/)\
\- [https://app-legacy.acryptos.com/deprecated/](https://app-legacy.acryptos.com/deprecated/)

These are links to deprecated vaults over the years. Your funds will still be there waiting for your withdrawal.

</details>

<details>

<summary>How do I check my yields and vault performance?</summary>

You can monitor your current deposits on our site via [https://debank.com/](https://debank.com/)

You can also click on the Withdraw button on each specific vault, to compare the changes from your initial deposits. More info [here](products/v3-aclm-vaults/ui-explanations.md#checking-your-yields).

You can also check past vault performance from the [History chart](products/v3-aclm-vaults/advanced-functions.md#graph-history) of each vault.

</details>

<details>

<summary>Why should I HODL the $ACS token?</summary>

Holding the $ACS token makes you part of the [DAO](dao/governance.md) governing ACryptoS, having ownership of the protocol and [treasury](dao/governance.md#treasury).

The $ACS token is a deflationary token, where there are no longer any emissions, and fees from our protocol go into [buybacks](dao/fees.md#acs-tokenomics) of the $ACS token, increasing its value over time.

</details>

<details>

<summary>Where can I buy $ACS?</summary>

Liquidity for $ACS is mainly on BSC. More info here.

</details>



***

{% hint style="warning" %}
_The FAQ below is outdated, and pending updates to our current products._
{% endhint %}

<details>

<summary>FAQ - legacy</summary>

## Trading/Listing, Supply Cap

### 1. What is ACS and what is ACSI? What are their core products?

* ACS is the native token of ACryptoS (connected with all the Vaults farming on PCS, Venus, Channels, MDEX, Unifi, Atlantis & DSG), while ACSI is the native token of the StableSwap & Acsi.Finance.
  * The core product of ACS is yield farming optimizers for multiple types of tokens.
  * The core products of ACSI are the [StableSwap](https://app.acryptos.com/stableswap/) (Stablecoin DEX) & [Acsi.Finance](https://app.acsi.finance/) (AMM).

### 2. Where is ACryptoS listed, where are ACS and ACSI traded?

ACryptoS is currently listed on:

* [Coinmarketcap](https://coinmarketcap.com/currencies/acryptos/)
* [Coingecko](https://www.coingecko.com/en/coins/acryptos)
* [Defistation](https://www.defistation.io/acryptos)
* [DappRadar](https://dappradar.com/binance-smart-chain/defi/acryptos)
* [MATH dApp Store](https://mathdapp.store)
* [Coinbase Prices](https://www.coinbase.com/price/acryptos)
* [TokenPocket Pro](https://www.tokenpocket.pro/)
* [Dfox - portfolio tracker](https://dfox.cc/)
* [Yieldwatch - farm and pool performance tracker](https://www.yieldwatch.net/)
* [Farm.army - farm and pool performance tracker](https://farm.army/)
* [SCV.finance - portfolio tracker](https://scv.finance/)
* [DeBank](https://debank.com/projects/bsc\_acryptos)
* [BitKeep Wallet](https://www.bitkeep.org/)

ACS is traded on:

* [Uniswap V3 (BSC)](https://app.uniswap.org/#/swap?inputCurrency=ETH\&outputCurrency=0x8888888888f004100c0353d657be6300587a6ccd\&chain=bnb)
* [Equilibre (Kava)](https://equilibrefinance.com/swap)

ACS V1 is traded on:

* [Acsi.Finance](https://app.acsi.finance/#/trade/0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE/0x4197C6EF3879a08cD51e5560da5064B773aa1d29) - **recommended to use**
* [1inch](https://app.1inch.io/#/r/0x5BD97307A40DfBFDBAEf4B3d997ADB816F2dadCC/BNB/ACS?network=56) - **recommended to use**
* [MDEX](https://bsc.mdex.com/#/swap?outputCurrency=0x4197C6EF3879a08cD51e5560da5064B773aa1d29)
* [OpenOcean](https://openocean.finance/classic)
* [Pancakeswap](https://exchange.pancakeswap.finance/#/swap?outputCurrency=0x4197C6EF3879a08cD51e5560da5064B773aa1d29)
* [DeBank](https://debank.com/swap?amount=1\&chain=bsc\&from=bsc\&to=0x4197c6ef3879a08cd51e5560da5064b773aa1d29)

ACSI is traded on:

* [Acsi.Finance](https://app.acsi.finance/#/trade/0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE/0x5b17b4d5e4009B5C43e3e3d63A5229F794cBA389) - **recommended to use**
* [1inch](https://app.1inch.io/#/r/0x5BD97307A40DfBFDBAEf4B3d997ADB816F2dadCC/ACS/ACSI?network=56) - **recommended to use**
* [OpenOcean](https://openocean.finance/classic)
* [Pancakeswap](https://exchange.pancakeswap.finance/#/swap?inputCurrency=0x4197C6EF3879a08cD51e5560da5064B773aa1d29\&outputCurrency=0x5b17b4d5e4009B5C43e3e3d63A5229F794cBA389)
* [DeBank](https://debank.com/swap?amount=1\&chain=bsc\&from=0x4197c6ef3879a08cd51e5560da5064b773aa1d29\&to=0x5b17b4d5e4009b5c43e3e3d63a5229f794cba389)

### 3. What is the maximum supply cap?

* The maximum supply cap for ACS is 1,888,888.
* The maximum supply cap for ACSI is 1,888,888.

### 4. Is there a buy-back program?

*   Yes. The system is designed to constantly buy-back ACS (using the withdrawal fee + the performance fee), and then those ACS are distributed to the acsACS holders.

    There are also constant buybacks for ACSI (using 50% of the swap fee from the StableSwap and 50% of the swap fees from Acsi.Finance), and then those ACSI are distributed to the acsACSI holders.

    You can read more [here](https://www.reddit.com/r/ACryptoS/comments/kth0v2/valuing\_users\_commitment\_buyback\_instead\_of\_burn/).

### 5. How many tokens are minted per day?

*   At start, there was a constant daily emission rate of \~3746 ACS tokens:

    \~2560 ACS to the farms

    \+33.33% to the ACS Vault (\~853)

    \+10% reward to the dev team (\~256)

    \+3% to the treasury (\~77)

    The genesis mining is \~8888 ACS.
* After the first ACS emission cut (15 Feb 2021), the ACS emission was reduced by 18.65%.
* After the second ACS emission cut (15 May 2021), the ACS emission was reduced by additional 18.65%.
* After the first ACSI emission cut (17 June 2021), the ACSI emission was reduced by \~32%, to match ACS' emissions.

### 6. Are the tokenomic models of ACS and ACSI sustainable?

* For ACS: the performance and withdrawal fees gained from providing the yield farming services to users are used to buy-back ACS from the market and then those ACS are redistributed to the ACS Vault Stakers. This ensures a sustainable future of ACS.
* For ACSI: 50% of the fees gained from the StableSwap and 50% of the fees gained from Acsi.Finance are used to buy-back ACSI from the market and then those ACSI are redistributed to the ACSI Vault Stakers. This ensures a sustainable future of ACSI.

### 7. What is the vision of ACS and ACSI?

* The vision of ACS is to be a long-term and sustainable yield optimizer on BSC, with a focus on safety.
* The vision of ACSI is to be the next-gen AMM on BSC, with new features to slash gas costs, super-charge capital efficiency, unlock arbitrage with zero-token starting capital, and open the door to custom AMMs.

## Security

### 1. Are the contracts behind a timelock?

* Yes, all contracts are behind a timelock. For more details, please refer to [Security & Risks](https://docs.acryptos.com/security-and-risks).

### 2. Are the contracts verified?

* Yes, all contracts have [verified and published source codes on BscScan](https://app.acryptos.com/contracts/).

### 3. Is the project audited?

Yes. The project has been audited. [Refer to here for the list of Audits](dao/security-and-risks.md#audits)

* [**Hacken - Complete**](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210331-Hacken-Complete.pdf) **(31 Mar 2021)**
* [**Certik - CAKE Vault Strategy**](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210324-Certik-StrategyACryptoSCakeTokenTokenV2.pdf) **-** [**1**](https://www.certik.org/projects/acryptos) **(24 March 2021)**
* [**Hacken - ACryptoS Farm V2**](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210218-Hacken-ACryptoSFarmV2.pdf) **-** [**1**](https://hacken.io/wp-content/uploads/2021/02/20210218-Hacken-ACryptoSFarmV2.pdf) **(18 Feb 2021)**
* [**DefiYield.info**](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210128-defiyield.info.pdf) **-** [**1**](https://defiyield.info/assets/pdf/ACryptoS.pdf) **(28 Jan 2021)**

## Fees

### 1. Is there a Deposit fee?

* No.

### 2. Is there a Stake fee?

* No.

### 3. What are the fees?

* There is a 0.1% withdrawal fee. This fee is applied on all vaults (except the ACS Vault and the ACSI Vault).
*   For the ACS Vault and the ACSI Vault, the withdrawal fee is 10% (applied only on the amount you withdraw).

    Example: If you have 1000 ACS in the ACS Vault, and you decide to withdraw 100 ACS, the fee will be 10 ACS.
* The performance fee and the workers fee are already included in the APY.

### 4. What are the harvest fees on the farms?

*   The harvest fee is 0.03 ACS on the ACS farms, and 0.06 ACSI on the ACSI farms.

    The harvest button appears after your Pending amount is more than 0.03 ACS (or more than 0.06 ACSI).

### 5. Which fees are visible and which are already included in the APR?

* The vault’s performance fee and workers fee are already included in the APY you see, so no need to do any math on that.
* You only need to be careful with the farms’ harvest fee (0.03 ACS , 0.06 ACSI), the vaults' withdrawal fee (0.1%), and the withdrawal fee on the ACS Vault & ACSI Vault (10%).

### 6. What are the fees on the StableSwap?

*   The exchange fees are set to 0.01% in the Corepool and 0.06% in the other Metapools, which is 5-30 times cheaper than the 0.3+% charged by all the other UniSwap and SushiSwap clones.

    All this is possible thanks to Curve’s [specialized algorithm tailored for trading of stablecoins and other pegged assets](https://www.curve.fi/stableswap-paper.pdf).

### 7. What are the fees on Acsi.Finance?

*   There are different pools on Acsi.Finance (up to 8 tokens in a pool), and there are different fees attached to every pool.

    You can check the fees with clicking on each pool.

## Technical and UI

### 1. What is the difference between Deposit (Vault) and Stake (Farm)?

* When you Deposit tokens to a Vault, the deposited tokens start to auto-compound right away.
* When you Stake those same tokens, you start earning ACS.

### 2. Is my ACS auto-compounding?

*   Yes, ACS auto-compounds in the ACS Vault.

    If you have Pending ACS in one of the other Vaults\&Farms, you first need to harvest those ACS and transfer them to the ACS Vault.

### 3. Is my ACSI auto-compounding?

*   Yes, ACSI auto-compounds in the ACSI Vault.

    If you have Pending ACSI in one of the other Vaults\&Farms, you first need to harvest those ACSI and transfer them to the ACSI Vault.

### 4. How the auto-compounding works (and what is the Workers tab)?

* Currently there is a bot that automatically harvests (compounds) each Vault.
*   There is also the [Workers tab](https://app.acryptos.com/worker/), where anyone can manually harvest each Vault (and get the associated fee).

    The Workers tab is just a backup, the normal user does not have to use it.

### 5. When does the ACS buy-back happen?

*   The ACS buy-back happens when the bot harvests the ACS Vault.

    When this happens, all the tokens gained from performance and withdrawal fees are first transferred to BNB, and then to ACS.

    Then the ACS is distributed to the ACS Vault stakers (acsACS holders).
* The same method is used for the ACSI buyback.

### 6. How do the Venus strategies work?

*   By supplying an asset and borrowing the same asset to resupply with.

    Example: Supply BNB, borrow BNB, supply more BNB, borrow more BNB, and repeat.

    With this method we are earning both supply and borrow rewards, with minimal liquidation risk as we are using a single asset.

### 7. Why does the APR on some Vaults show weird numbers?

*   The UI shows the average APR of the last 3 days.

    So if a Vault is new, the numbers could be off.

### 8. I cannot find the “harvest” or “withdraw” button, where are they?

* The User interface (UI) is dynamic. The harvest button appears after you have at least 0.03 ACS Pending for harvest.
* If your assets are Staked, the Withdraw button appears after the Unstake.

### 9. What is ACS4USD/ACS4VAI/ACS4UST?

*   When you deposit Stable coins to the StableSwap, you receive ACS4\_\*\_ tokens as a receipt/proof of deposit.

    Then you can stake those ACS4\_\*\_ tokens in the ACSI farms to earn ACSI.

### 10. What is the difference between APR and APY?

* APR reflects the simple interest rate over a year’s time (APR/365), while APY describes the rate with the effect of compounding.

## Governance and Voting

### 1. Is there a treasury?

* Yes. A treasury was formed to fund anything that adds value to the protocol, taking up to 3% of ACS & ACSI emissions.

### 2. What is the main goal of the treasury?

* The treasury funds will be used to add value/improve the project (marketing/pr/administration/management/audits/etc).

### 3. Who controls the treasury?

* The treasury is controlled via governance.

### 4. Who can vote?

* ACS held in the ACS Vault and ACSI held in the ACSI Vault are our governance tokens. Voting weight is measured in ACS, using the prevailing ACS-ACSI exchange rate.

### 5. Where do I vote?

* You can vote on [the governance platform](https://vote.acryptos.com/#/acryptos/all).

### 6. Who can create a new vote/proposal?

* Anyone who holds at least 88 ACS (or the equivalent in ACSI).

### 7. Which governance platform is used for voting?

* We are using the well-established gasless [governance client](https://snapshot.page) by Snapshot Labs.

</details>

