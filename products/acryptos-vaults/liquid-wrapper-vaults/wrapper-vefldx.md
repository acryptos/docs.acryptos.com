# Flair DEX veFLDX

## How It Works

[Flair DEX](https://app.flairdex.xyz/) $FLDX

* They have a 2.5X [Boost function](https://docs.flairdex.xyz/core-concepts/rewards#boosting) for their LP farms. If a user stakes $FLDX as a veNFT, locking it for a period of time, they will receive Boosts on the LP farms they stake in.
* The larger the veNFT they have, the more they will be able to Boost the LP farms.

———

### 1️⃣ autoCompunding vaults for Liquidity Pool farms

* These vaults collect $FLDX emissions from the farm, and autoCompound them back into the LP, increasing the number of tokens in the LP
* The veNFT in the Liquid veFLDX Vault (explained [below](../../../acryptos-vaults/acryptos-vaults/liquid-wrapper-vaults/#2-liquid-vesliz-vault-acssliz)) will Boost the APY for these vaults, up to 2.5X

Examples:

* User A forms a AVAX-USDC LP, and farms it for 50% APR, manually harvesting the $FLDX rewards every few days. User A has no Boosted rewards because he doesn't lock $FLDX for any veFLDX
* User B forms a AVAX-USDC LP, and stakes in our AVAX-USDC Vault. The $FLDX rewards are autoCompounded few times a day, swapping $FLDX to AVAX and USDC, forming more AVAX-USDC LP, and adding on to the original stake. User B gets 125% APR (2.5X Boosted rewards) even if he doesn't lock $FLDX for veFLDX.

TL/DR 👉Users can autoCompound their LP with Boosted rewards, without needing to lock $FLDX to veFLDX themselves.

### 2️⃣ Liquid veFLDX Vault (acsFLDX)

* Users stake their $FLDX in the vault, getting a acsFLDX receipt token, and get benefits as if they locked veFLDX themselves (trading fees/bribes/rebases etc.). Our strategy then locks the $FLDX for max period, getting max veFLDX voting power.
* 50% of Boosted rewards from ALL our LP Vaults, are rewarded to acsFLDX (veFLDX Vault) holders
* This veFLDX Vault allows users to withdraw $FLDX at any time, where otherwise their veFLDX would be locked for 4 years

_\*Note: Withdrawals are subject to available $FLDX in the Vault Reserves. Reserves are constanly topped up from above-mentioned sources (bribes/Boost Rewards etc.). Vault Strategy is based on our Liquidizer Vault (one of our other unique strategies, more info_ [_here_](../../../acryptos-vaults/acryptos-vaults/liquidizer-vaults.md)_)_

TL/DR 👉 Users stake their $FLDX, gets full locking benefits without locking, gets rewards APY from all our LP Vaults on Flair DEX

The more $FLDX staked in the veFLDX Vault, the higher the Boosted APY for the LP vaults↩️

The more the LP vaults gain TVL, the more rewards go to the veFLDX Vault↩️

### 3️⃣ acsFLDX-FLDX LP vault

* Users can pair their acsFLDX token (Liquid veFLDX Vault receipt) with $FLDX, forming an LP
* The voting power from the single-token veFLDX Vault will be directed to the acsFLDX-FLDX LP farm _\*voting strategy might be adjusted after initial launch period, based on TVL and APY_
* Based on the weekly voting %, the farm receives $FLDX emissions.
* Users can form the LP and stake in our acsFLDX-FLDX Vault, autoCompounding more of acsFLDX-FLDX
* This acsFLDX-FLDX LP provides another method for users to exit their acsFLDX position back to $FLDX

TL/DR 👉 Users get max APY by staking in Liquid veFLDX Vault, then using the receipt acsFLDX token to stake further in acsFLDX-FLDX Vault

***

## Steps:

Investing in FLDX-acsFLDX Vault

1. Buy $FLDX on https://app.flairdex.xyz/swap
2. Stake $FLDX in our [veFLDX Vault](https://app.acryptos.com/vaults/43114/0x2Dd5a62a5D4E4D20622061C823f9648E3078012d), and get acsFLDX receipt token
3. Form FLDX-acsFLDX LP at https://app.flairdex.xyz/liquidity
4. Stake in our [FLDX-acsFLDX Vault](https://app.acryptos.com/vaults/43114/0x567c7c67d3e8C4805eff56B8F143753fa1337A23)

***

### Additional Notes:

The above vaults can be used independent of each other.

Withdrawal fees: 0.1%
