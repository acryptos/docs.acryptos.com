---
description: >-
  The following explains sections of the UI, showing detailed info about each of
  the vaults.
---

# UI Explanations

## Vault Header APY

APY displayed on the header is pulled from the last 8th compound of the vault. (see below)

![Vault Header APY](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/ACLM%20-%20Vault%20Header%20APY.png)

Expanding the "Advanced" section, you can find a table displaying the Historical APY of this vault "180%" can be seen from the 8th row (3rd column) - Cumulative

## Checking your Yields

Click on the Withdraw tab, tap on full withdrawal amount and check the amount of tokens received.

Do not execute the withdrawal transaction.

***

## Advanced

### Historical APY

![Historical APY](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/ACLM%20-%20APY%20History.png)

Explanation of the Historical APY:

* Each line refers to one of the latest rebalancing/compounding
* For the 8th line, it can be explained as:
  * the compound was 1.05 days ago
  * the APY achieved between 0.96 - 1.05 days ago is 149%
  * the Cumulative (Total) APY achieved between now and 1.05 days ago is 180%
  * the Impermanent Loss (IL) between 0.96 - 1.05 days ago was -24%
  * the Cumulative IL between now and 1.05 days ago is positive 0.64% (gains instead of IL)

### Chart - u3i

We have developed a chart to help users visualize the current distribution of liquidity on a specific LP, the current trading price, and the active liquidity managed by our strategies.

Expanding the "Advanced" section under each ACLM vault, you can find a "u3i" link.&#x20;

<img src="https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/u3i%20-%20Arbitrum%20USDT-USDC%20240228.png" alt="Screenshot of managed USDT-USDC (Arbitrum) active liquidity %" data-size="original">

* blue bar indicates managed liquidity on ACryptoS
* grey bars indicate other providers
* large amount of under-utilized liquidity can be seen from the grey bars

### Graph - History

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
