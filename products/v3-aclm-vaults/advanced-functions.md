# Advanced Functions

## Chart - u3i

We have developed a chart to help users visualize the current distribution of liquidity on a specific LP, the current trading price, and the active liquidity managed by our strategies.

Expanding the "Advanced" section under each ACLM vault, you can find a "u3i" link.&#x20;

<img src="https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/u3i%20-%20Arbitrum%20USDT-USDC%20240228.png" alt="Screenshot of managed USDT-USDC (Arbitrum) active liquidity %" data-size="original">

* blue bar indicates managed liquidity on ACryptoS
* grey bars indicate other providers
* large amount of under-utilized liquidity can be seen from the grey bars

## Graph - History

Expanding the "Advanced" > "History" section, you will see a graph indicating the historical performance of this ACLM vault.

![History Graph](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/History%20Graph%20-%20VELA-ETH.jpg)

The above is a graph for the VELA/ETH vault on Arbitrum Uniswap V3.

* blue line is the APY gained
* cyan line is the IL
* green line is the nett APY

To understand this graph, we look at the green line to find out the actual APY received.

* the graph shows a period from 18 Nov to 4 Dec 2023
* Green lines shows 27.12% gained from 18 Nov to 4 Dec (18 days)
* Converted to APR 27.12% / 18 days \* 365 days = 549%
* Converted to APY = 23155%

\*_The history graph pulls data from the last 188 harvests of the vault._

***

## ACryptos - Keeper

We developed a Keeper bot, to automate various vault functions based on external triggers. This ensures that our vaults function at the highest effectiveness, and minimizes the potential IL of the vaults.

***

## User Triggers

### Harvest Vault

Triggers a rebalance of the vault, by harvesting incentives, swapping them and compounding them back into the vault. Harvesting consumes gas fees.

Triggering the harvest gives the user harvester fees (0.3% of the incentives) to offset the gas fees, and also as an incentive to decentralize the rebalancing function, where users will always have an incentive to rebalance the vault in the long run.

Harvester rewards are received in the form of the vault acsXYZ token.

{% hint style="info" %}
It is not required to press on the "Harvest Vault" function. Our automation processes will handle this in the back end. Only do this if you want to earn the harvester fees, or if you would like to compound the rewards before exiting the vault.
{% endhint %}

### Harvest Merkl Rewards

Triggers a harvest of pending Merkl Rewards, and compounding them back into the vault. Harvesting consumes gas fees.
