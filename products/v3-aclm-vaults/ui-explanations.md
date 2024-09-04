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

0.05% refers to the swap fee rate on the underlying pool.

## Historical APY

![Historical APY](https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/ACLM%20-%20APY%20History.png)

Explanation of the Historical APY:

* Each line refers to one of the latest rebalancing/compounding
* For the 8th line, it can be explained as:
  * the compound was 1.05 days ago
  * the APY achieved between 0.96 - 1.05 days ago is 149%
  * the Cumulative (Total) APY achieved between now and 1.05 days ago is 180%
  * the Impermanent Loss (IL) between 0.96 - 1.05 days ago was -24%
  * the Cumulative IL between now and 1.05 days ago is positive 0.64% (gains instead of IL)

***

<figure><img src="https://raw.githubusercontent.com/acryptos/docs.acryptos.com/master/images/Docs%20-%20UI%20categories.png" alt=""><figcaption></figcaption></figure>

What's LP-A? USD-B? That's our categorization of vaults. Learn more [here](../../quick-start-guide.md#categories).

***

## Checking your Yields

Click on the Withdraw tab, tap on full withdrawal amount and check the amount of tokens received.

_\*do not execute the withdrawal transaction_

***

## Error Messages

{% hint style="warning" %}
Prices are volatile. Please try again later.
{% endhint %}

If you see this notice while depositing, please wait for some time before trying again. These are [preventative measures](strategies.md#exploit-risk-mitigations) for vault safety when prices are volatile.
