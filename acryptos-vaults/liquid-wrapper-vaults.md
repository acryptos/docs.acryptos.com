# Liquid Wrapper Vaults

Our Liquid Wrapper Vaults are a set of vaults specially designed to work with ve(3,3) DEXs, allowing liquidity for otherwise locked native tokens, and providing Boosted yields for users. These vaults work cohesively together to form a positive flywheel.

### Benefits:
- helping ve(3,3) protocols lock more of their native tokens to veNFTs
- allowing users to farm higher APY with their tokens without the need to invest in native token veNFTs

## How It Works

_(Using one of our partners, [SolidLizard](https://solidlizard.finance/) $SLIZ as an example)_

They have a 2.5X [Boost function](https://solidlizard.gitbook.io/solidlizard/how-to-use-the-boost-calculator) for their LP farms. If a user stakes $SLIZ as a veNFT, locking it for a period of time, they will receive Boosts on the LP farms they stake in.

The larger the veNFT they have, the more they will be able to Boost the LP farms. 

———

### 1️⃣ autoCompunding vaults for Liquidity Pool farms
- These vaults collect $SLIZ emissions from the farm, and autoCompound them back into the LP, increasing the number of tokens in the LP
- The veNFT in the Liquid veSLIZ Vault (explained [below](../acryptos-vaults/liquid-wrapper-vaults#2-liquid-vesliz-vault-acssliz)) will Boost the APY for these vaults, up to 2.5X

Examples:
- User A forms a ETH-ARB LP, and farms it for 50% APR, manually harvesting the $SLIZ rewards every few days. User A has no Boosted rewards because he doesn't lock $SLIZ for any veSLIZ
- User B forms a ETH-ARB LP, and stakes in our ETH-ARB Vault. The $SLIZ rewards are autoCompounded few times a day, swapping $SLIZ to ETH and ARB, forming more ETH-ARB LP, and adding on to the original stake. User B gets 125% APR (2.5X Boosted rewards) even if he doesn't lock $SLIZ for veSLIZ.

TL/DR 👉Users can autoCompound their LP with Boosted rewards, without needing to lock $SLIZ to veSLIZ themselves.

### 2️⃣ Liquid veSLIZ Vault (acsSLIZ)
- Users stake their $SLIZ in the vault, getting a acsSLIZ receipt token, and get benefits as if they locked veSLIZ themselves (trading fees/bribes/rebases etc.). Our strategy then locks the $SLIZ for max period, getting max veSLIZ voting power.
- 50% of Boosted rewards from ALL our LP Vaults, are rewarded to acsSLIZ (veSLIZ Vault) holders
- This veSLIZ Vault allows users to withdraw $SLIZ at any time, where otherwise their veSLIZ would be locked for 4 years

_*Note: Withdrawals are subject to available $SLIZ in the Vault Reserves. Reserves are constanly topped up from above-mentioned sources (bribes/Boost Rewards etc.). Vault Strategy is based on our Liquidizer Vault (one of our other unique strategies, more info [here](../acryptos-vaults/liquidizer-vaults.md))_

TL/DR 👉 Users stake their $SLIZ, gets full locking benefits without locking, gets rewards APY from all our LP Vaults on SolidLizard

The more $SLIZ staked in the veSLIZ Vault, the higher the Boosted APY for the LP vaults↩️

The more the LP vaults gain TVL, the more rewards go to the veSLIZ Vault↩️

### 3️⃣ acsSLIZ-SLIZ LP vault
- Users can pair their acsSLIZ token (Liquid veSLIZ Vault receipt) with $SLIZ, forming an LP
- The voting power from the single-token veSLIZ Vault will be directed to the acsSLIZ-SLIZ LP farm
_*voting strategy might be adjusted after initial launch period, based on TVL and APY_
- Based on the weekly voting %, the farm receives $SLIZ emissions.
- Users can form the LP and stake in our acsSLIZ-SLIZ Vault, autoCompounding more of acsSLIZ-SLIZ
- This acsSLIZ-SLIZ LP provides another method for users to exit their acsSLIZ position back to $SLIZ

TL/DR 👉 Users get max APY by staking in Liquid veSLIZ Vault, then using the receipt acsSLIZ token to stake further in acsSLIZ-SLIZ Vault

---

### Additional Notes:

The above vaults can be used independent of each other.

Withdrawal fees: 0.1%
