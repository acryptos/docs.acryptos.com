---
description: >-
  ACS and ACSI are distributed via ACryptoS Farms to incentivise liquidity
  providers and share a stake in the protocol with our users.
---

# ACryptoS Farms

Most Vaults and StableSwap pools will have a corresponding Farm where they can be staked to earn ACS or ACSI. Be sure to stake in the Farm after depositing into a Vault or StableSwap pool.

## ACS Farms V2

The SFP-BNB Vault&Farm and LTC Vault&Farm were the first Vaults on V2 to go live on 10 Feb 2021. We plan to migrate all ACS Farms to V2 eventually, this will be announced at a later date with ample notice.

* Staking and un-staking no longer triggers a harvest.
* ACS Vault holdings is used to boost rewards up to 2.5X.

### ACS Rewards Boost

In V2, ACS Vault holdings are used to boost ACS rewards by up to 2.5X. The amount of boost is determined via the following formula:

1.5 \* \[% user's share of acsACS\] \* \[TVL in Farm\]

Example: User deposits 20 LTC in Vault&Farm, there is 1500 LTC in the farm in total, and user has 1% share of the ACS Vault. His available boost is 1500 \* 1.5 \* 1% = 22.5 LTC, so a share of 20 + 22.5 = 42.5 LTC will be used to calculate his ACS Rewards. If he deposits only 1 LTC, it will be boosted to the maximum 2.5X of 2.5 LTC. If he deposits 100 LTC, it will be boosted to 100 + 22.5 = 122.5 LTC.

User's boost is updated on every stake/un-stake/harvest.

### **User Interface**

**Current Boost**: The current boost you are getting in the farm from your ACS Vault holdings.  
**Future Boost**: The boost you will get after you stake/un-stake/harvest. Pressing 'Force' will update this boost manually.  
**For 2.5X**: The amount of vaulted ACS you need to get the maximum boost on your current Farm stake.  
**2.5X On First**: The amount you can stake in the Farm that will get the maximum boost based on your current vaulted ACS.  


