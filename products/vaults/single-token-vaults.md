# Supply-Borrow Leveraged Vaults

![](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/Guide%20-%20Single-Token%20Looping.jpg)

Single token vaults are one of the most unique offerings at ACryptoS. We partner with and build on lending protocols, using our smart contract strategies to automatically leverage the same token.

By borrowing and supplying the same token in a number of loops, users earn Supply and Borrow APY multiple times, up to 7.6X the initial APY.&#x20;

{% hint style="success" %}
Our strategy helps users get much higher yields for their tokens, and also increases the deposits and utilizations of lending markets.
{% endhint %}

There is zero liquidation risk in our strategy, as it is using the same token for supplying and borrowing. Price movements of the token do not result in liquidations. Understand how it works [here](../../dao/security-and-risks.md#risk-liquidation-risks).

## Vault Benefits

1. auto-Compounding\
   \- vaults compound automatically through our smart contract strategy\
   \- staked tokens increase over time
2. no IL (impermanent loss)\
   \- single token staking, no impermanent loss as per LP farming
3. automated, no harvesting required\
   \- APY is in staked tokens, not from farming emission tokens
4. safety-first\
   \- we filter and partner with quality protocols, putting our priorities on user fund safety\
   \- no security issues since 2020 launch

***

## Protocols

Vaults are built on the following protocols

* Venus (BSC)
* Moonwell (Optimism, Base, Moonbeam, Moonriver)
* Mendi (Linea)
* Lodestar (Arbitrum)
* Benqi (Avalanche) - sAVAX
* Stargate (Kava) - S\*USDt

***

## Advanced Functions

<figure><img src="../../.gitbook/assets/single-token harvest vault.png" alt="" width="563"><figcaption></figcaption></figure>

**"Reward"** amount refers to the number of vault tokens that a user will receive when the **"Harvest Vault"** function is triggered. These are called harvester fees (a set % of the pending rewards), with the % varied depending on different vaults _(0.03% in this case here)._ These fees serve as an incentive to compensate the gas fees used for compounding the vault.

{% hint style="success" %}
Harvester rewards are received in the form of the vault acsXYZ token.
{% endhint %}

_This is also to ensure the sustainability of our vaults, where users will always have an incentive to keep the vault compounding in the long run as long as there is TVL and fees._

### Harvest Vault

The **"Harvest Vault"** function triggers a rebalance of the vault, by harvesting incentives, swapping them and compounding them back into the vault. The function also checks for the optimum leverage ratio based on the supply/borrow % of the token's market in the underlying lending protocol, rebalancing the leverage ratio as needed.

{% hint style="info" %}
**Harvesting consumes gas fees.**

It is not required to press on the "Harvest Vault" function. Our automation processes will handle this in the back end.

Only do this if you want to earn the harvester fees, or if you would like to compound the rewards before exiting the vault.
{% endhint %}

### Trigger Rebalance

<figure><img src="../../.gitbook/assets/single-token trigger rebalance.png" alt="" width="563"><figcaption></figcaption></figure>

The **"Trigger Rebalance"** function checks for the optimum leverage ratio for this vault, and rebalances the supply/borrow loops as needed to achieve the highest APY for the vault. It works similarly to the "Harvest Vault" function mentioned above, except it does not trigger a harvest of fees or compound of the vault.

Harvesting consumes gas fees.

{% hint style="info" %}
**Harvesting consumes gas fees.**

It is not required to press on the "Trigger Rebalance" function. Our automation processes will handle this in the back end.
{% endhint %}

