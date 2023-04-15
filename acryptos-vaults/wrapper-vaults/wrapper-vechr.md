# Chronos Liquid Wrapper Vault (acsCHR)

## How It Works


———

### 1️⃣ autoCompunding vaults for Liquidity Pool farms
- These vaults collect $CHR emissions from the farm, and autoCompound them back into the LP, increasing the number of tokens in the LP
- The veNFT in the Liquid veCHR Vault (explained [below](../acryptos-vaults/liquid-wrapper-vaults#2-liquid-vesliz-vault-acssliz)) will Boost the APY for these vaults, up to 2.5X

Examples:
- User A forms a ETH-ARB LP, and farms it for 50% APR, manually harvesting the $CHR rewards every few days. User A has no Boosted rewards because he doesn't lock $CHR for any veCHR
- User B forms a ETH-ARB LP, and stakes in our ETH-ARB Vault. The $CHR rewards are autoCompounded few times a day, swapping $CHR to ETH and ARB, forming more ETH-ARB LP, and adding on to the original stake. User B gets 125% APR (2.5X Boosted rewards) even if he doesn't lock $CHR for veCHR.

TL/DR 👉Users can autoCompound their LP with Boosted rewards, without needing to lock $CHR to veCHR themselves.

### 2️⃣ Liquid veCHR Vault (acsCHR)
- Users stake their $CHR in the vault, getting a acsCHR receipt token, and get benefits as if they locked veCHR themselves (trading fees/bribes/rebases etc.). Our strategy then locks the $CHR for max period, getting max veCHR voting power.
- 50% of Boosted rewards from ALL our LP Vaults, are rewarded to acsCHR (veCHR Vault) holders
- This veCHR Vault allows users to withdraw $CHR at any time, where otherwise their veCHR would be locked for 4 years

_*Note: Withdrawals are subject to available $CHR in the Vault Reserves. Reserves are constanly topped up from above-mentioned sources (bribes/Boost Rewards etc.). Vault Strategy is based on our Liquidizer Vault (one of our other unique strategies, more info [here](../acryptos-vaults/liquidizer-vaults.md))_

TL/DR 👉 Users stake their $CHR, gets full locking benefits without locking, gets rewards APY from all our LP Vaults on SolidLizard

The more $CHR staked in the veCHR Vault, the higher the Boosted APY for the LP vaults↩️

The more the LP vaults gain TVL, the more rewards go to the veCHR Vault↩️

### 3️⃣ acsCHR-CHR LP vault
- Users can pair their acsCHR token (Liquid veCHR Vault receipt) with $CHR, forming an LP
- The voting power from the single-token veCHR Vault will be directed to the acsCHR-CHR LP farm
_*voting strategy might be adjusted after initial launch period, based on TVL and APY_
- Based on the weekly voting %, the farm receives $CHR emissions.
- Users can form the LP and stake in our acsCHR-CHR Vault, autoCompounding more of acsCHR-CHR
- This acsCHR-CHR LP provides another method for users to exit their acsCHR position back to $CHR

TL/DR 👉 Users get max APY by staking in Liquid veCHR Vault, then using the receipt acsCHR token to stake further in acsCHR-CHR Vault

---

## Steps:
Investing in CHR-acsCHR Vault

1) Buy $CHR on https://solidlizard.finance/swap

2) Stake $CHR in our [veCHR Vault](https://app.acryptos.com/vaults/42161/0x16C4BA98623a1B05d35b9923fB00E9fE02D0B47f), and get acsCHR receipt token

3) Form CHR-acsCHR LP at https://solidlizard.finance/liquidity

4) Stake in our [CHR-acsCHR Vault](https://app.acryptos.com/vaults/42161/0x61A34758576D651643A90838f3eCF86e8680874D)

---

### Additional Notes:

The above vaults can be used independent of each other.

Withdrawal fees: 0.1%
