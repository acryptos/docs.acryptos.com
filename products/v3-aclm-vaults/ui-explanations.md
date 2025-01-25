---
description: >-
  The following explains sections of the UI, showing detailed info about each of
  the vaults.
---

# UI Explanations

## Main Page

Dapp: [https://app.acryptos.com/](https://app.acryptos.com/)

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Filtering functions</p></figcaption></figure>

* **"ACLM"**  shows all our vaults that utilize our Advanced Conc. Liquidity Manager strategies.
* **"Single"** shows all our vaults that are built on lending protocols, using looped strategies, with no liquidation risks and no IL.&#x20;

{% hint style="info" %}
Find out more about ACLM and Single-Token Vaults differences [here](../../quick-start-guide.md#vault-comparisons).

Explanations and breakdowns on categories of eg. LP-A, USD-B, etc can be found [here](../../quick-start-guide.md#categories).
{% endhint %}

***

## Vault Details

Clicking into any of the vaults from the Main Page, brings you to the individual Vault Details page.

<figure><img src="https://raw.githubusercontent.com/acryptos/docs.acryptos.com/refs/heads/master/images/ACLM%20-%20Vault%20Header%20APY%20v2.png" alt=""><figcaption><p>Vault Header APY</p></figcaption></figure>

The <mark style="color:orange;">0.01%</mark> on the header refers to the swap fee rate on the underlying pool, generally varying from 0.01% to 0.30%, or even up to 1.00%. In this example, this vault manages the 0.01% swap fee USDC/USDT pool on UniswapV3 (Base)

The <mark style="color:green;">amount of tokens highlighted in green</mark>, is the ratio of USDC and USDT currently managed in our vault. _The ratio will constantly change as the vault rebalances._ The ratio does not concern users as they may deposit in **any ratio between the 2 tokens**, or even do **single-sided deposits**. The vault strategy will rebalance as neccessary.

The <mark style="color:yellow;">APY</mark> displayed on the header, is an average of the last 3 days APY, pulled the last 8 compounds of the vault. (see [Historical APY](ui-explanations.md#historical-apy) below)

***

### Additional Merkl rewards

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Additional incentives distributed via Merkl</p></figcaption></figure>

Certain pools may be allocated incentives via grants or reward campaigns from time to time. Our vault strategies are optimized to

* harvest these additional rewards (eg. UNI, ARB, etc.)
* converting them to the tokens managed in the vault (in this example: WBTC and tBTC)
* and autocompounding them back into the vault

{% hint style="success" %}
This automated process increases the APY for users, and lessens the hassle for users to harvest the Merkl rewards themselves.&#x20;
{% endhint %}

Clicking on the <mark style="color:green;">green Merkl reward button</mark>, brings you to the Merkl rewards page, where you can monitor how much rewards are being distributed, and how long more the campaign will run for. You may also check the performance of our vaults on the Leaderboard for the Merkl rewards page.

Here's a short [tweet](https://x.com/acryptosdao/status/1817912082337239123) indicating our performance on one of the vaults.

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Our USDC/USDT vault in the #1 position on Merkl.</p></figcaption></figure>

{% hint style="info" %}
The contract for each of the vaults can be found in the [Advanced ](ui-explanations.md#advanced)section, under Contracts - Vault.
{% endhint %}

#### Notes:

* the displayed APR in the <mark style="color:green;">green Merkl reward button</mark> is via Merkl's API (Total Rewards/TVL)
* our vaults typically achieve higher APY as our strategies are designed to be more concentrated
* APY displayed in our header has already factored in the additional incentives

***

### Error Messages while Depositing

{% hint style="warning" %}
Prices are volatile. Please try again later.
{% endhint %}

If you see this notice while depositing, please wait for some time before trying again. These are [preventative measures](strategies.md#exploit-risk-mitigations) for vault safety when prices are volatile.

***

### Checking your Yields

1. Click on the Withdraw tab
2. Tap on the "Balance" for the full withdrawal amount
3. Check the amount of tokens you are estimated to receive\
   &#xNAN;_\*do not execute the withdrawal transaction_
4. Compare the tokens received with your initial deposits.

***

## Advanced

Expanding the **"Advanced"** section under the basic Vault Details, opens up a large number of sections that show the Historical APY, detailed contracts, backend workings of the vault, %-managed-liquidity charts, past-performance graphs, etc.

### Harvesting / Compounding

This block shows the date and time that this vault was last harvested, along with additional triggers that users may use to trigger compounding of rewards. Read more about these triggers [here](advanced-functions.md#user-triggers).

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Compounding functions.</p></figcaption></figure>

***

### Historical APY

The following block displays the Historical APY of an example vault.

![Historical APY](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/ACLM%20-%20APY%20History.png)

**Explanation of the Historical APY:**

* Each line refers to one of the latest harvesting/rebalancing/compounding
* For the 8th line, it can be explained as:
  * the compound was 1.04 days ago
  * the APY achieved between 0.95 - 1.04 days ago is 149%
  * the Cumulative (Total) APY achieved between now and 1.04 days ago is 180%
  * the Impermanent Loss (IL) between 0.95 - 1.04 days ago was -24%
  * the Cumulative IL between now and 1.04 days ago is positive 0.64% (gains instead of IL)

***

### Advanced Functions

The **"u3i"** found under **"Advanced Strategy"** opens up a chart where users can find out how much % of liquidity is being managed by our ACryptoS strategy for that specific pool. Details [here](advanced-functions.md#chart-u3i).

Scrolling to the bottom and expanding **"History"**  opens up a graph where users can check the performance of this vault over a period of time. Details [here](advanced-functions.md#graph-history).
