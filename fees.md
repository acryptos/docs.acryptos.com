# Tokenomics & Fees

## ACS Tokenomics

**ACS rewards distributed to ACS Farms: 0.088888 888888 888888 ACS/block** \(~ 2560 ACS/day\)  
**+33.33% distributed to ACS holders via ACS Vault  
+10% reward to ACryptoS Dev Team**  
Total ~3669 ACS/day  
**Up to 3% of supply may be minted for ACryptoS Treasury**

Maximum supply cap at 1,888,888 ACS.

All parameters may be adjusted in future via governance.

### ACS Vault

Withdrawal fee: 10% \(distributed to ACS holders - remains in vault\)

ACS Vault tokens \(acsACS\) are non-transferrable. You will have to withdraw ACS to transfer.

### All Vaults \(except ACS and ACSI Vault\)

**Withdrawal fee: 0.5%** \(used to buy ACS and distributed to ACS holders via ACS Vault\)

**Performance fee: 5% of gains harvested**  
Up to 0.5% to strategy creator.  
Remainder used to buy ACS and distributed to ACS holders via ACS Vault.

### All Vaults

**Harvester fee: 0.3% of gains harvested**  
Paid to Workers to offset gas fees.

### ACS Farms

**Transaction fee: 0.5 ACS** \(max\)  
**Fee will not exceed user's pending ACS rewards.**  
Will be levied on any harvest, stake or un-stake. Fee will be deducted from user's pending ACS rewards, and remainder will be transferred to user.  
Farm transaction fees are distributed to ACS holders via ACS Vault.

### ACS Farms V2

The SFP-BNB Vault&Farm and LTC Vault&Farm will be the first \(and only\) Vaults on V2 to start on 10 Feb 2021. We plan to migrate all ACS Farms to V2 eventually, this will be announced at a later date with ample notice.

* Staking and un-staking no longer triggers a harvest.
* ACS Vault holdings is used to boost rewards up to 2.5X.

**Harvest fee: 0.5 ACS** \(max\)  
**Fee will not exceed user's pending ACS rewards.**  
Fee will be deducted from user's pending ACS rewards, and remainder will be transferred to user.  
Farm harvest fees are distributed to ACS holders via ACS Vault.

#### ACS Rewards Boost

In V2, ACS Vault holdings are used to boost ACS rewards by up to 2.5X. The amount of boost is determined via the following formula:

1.5 \* \[% user's share of acsACS\] \* \[TVL in Farm\]

Example: User deposits 20 LTC in Vault&Farm, there is 1500 LTC in the farm in total, and user has 1% share of the ACS Vault. His available boost is 1500 \* 1.5 \* 1% = 22.5 LTC, so a share of 20 + 22.5 = 42.5 LTC will be used to calculate his ACS Rewards. If he deposits only 1 LTC, it will be boosted to the maximum 2.5X of 2.5 LTC. If he deposits 100 LTC, it will be boosted to 100 + 22.5 = 122.5 LTC.

User's boost is updated on every stake/un-stake/harvest.

## ACSI Tokenomics

**ACSI rewards distributed to ACSI Farms: 0.088888 888888 888888 ACSI/block** \(~ 2560 ACSI/day\)  
**+33.33% distributed to ACSI holders via ACSI Vault  
+10% reward to ACryptoS Dev Team**  
Total ~3669 ACSI/day

Currently no cap on maximum supply.  
All parameters may be adjusted in future via governance.

### ACSI Vault

Withdrawal fee: 10% \(distributed to ACSI holders - remains in vault\)

ACSI Vault tokens \(acsACSI\) are non-transferrable. You will have to withdraw ACSI to transfer.

### ACSI Farms

**Harvest fee: 5 ACSI** \(max\)  
**Fee will not exceed user's pending ACSI rewards.**  
Fee will be deducted from user's pending ACSI rewards, and remainder will be transferred to user.  
Farm harvest fees are distributed to ACSI holders via ACSI Vault.

### StableSwap

**Exchange fee: 0.04% \(ACS4USD base-pool\) / 0.06% \(meta-pools\)**  
50% of the exchange fee is used to buy and distribute ACSI to ACSI holders via ACSI Vault. Remainder is earned by liquidity providers in the pool.

