---
description: >-
  The first native liquid staking BNB product on BSC, featuring fully automated,
  on-chain de-centralized operations.
---

# BNB Native Liquid Staking

The **first** _**native**_ liquid staking BNB product on BSC, launched on 9 Feb 2023.

Featuring fully automated, on-chain de-centralized operations, utilizing the [new native staking system contract on BSC](https://bscscan.com/address/0x0000000000000000000000000000000000002001), implemented via [BEP-153](https://github.com/bnb-chain/BEPs/blob/master/BEP153.md).

The use of the native staking system contract means that all operations between BSC and BC are performed on-chain, providing a transparent and secure process.

This Vault is a [Liquidizer Vault](acryptos-vaults/liquidizer-vaults.md) and a reserve of BNB is kept on BSC to enable immediate withdrawals. When reserves run low, an undelegation is triggered on BC to automatically top them up, subject to the 7-day unbonding period.

## Verification Reference

First delegation:\
[Deposit on BSC](https://bscscan.com/tx/0xd48b7205a0bed3945f166b59474b5d8e7f54431fac83d2676e17baa7f8c1b940#eventlog) -> [Delegate on BC](https://explorer.bnbchain.org/tx/80D6CFDF4535D4D6BC1DEC55BBE2A6577BF357767A8F34FE9DE3F79A25F4A420) -> [Delegate ACK on BSC](https://bscscan.com/tx/0x7ca0e0d5f73c32e0e120fbec4948c7b10da7fc9757f3b2b2d49dd320fa02a0a7#eventlog)

Reward address on BC: [bnb19ws83p95z4f4tf2u0l03ehp03aa3ckrfjly09q](https://explorer.bnbchain.org/address/bnb19ws83p95z4f4tf2u0l03ehp03aa3ckrfjly09q)

Note: reward accumulates on BC and gets sent back to BSC when it reaches > \~1 BNB.

Delegate address on BC: [bnb1q0v3ej7fq603nl2vglram26egy5xmwt6q6gsgn](https://explorer.bnbchain.org/address/bnb1q0v3ej7fq603nl2vglram26egy5xmwt6q6gsgn)

Note: Explorer does not show delegations on delegate address page, but you can verify them from the validators' pages - reward address -> staking tab -> any validator -> delegators tab -> scroll and search for delegate address

First staking reward:\
[Reward received on BSC](https://bscscan.com/tx/0xdb5b63de7fe3a09d0e7ddcc30cf85c3e6fc27c7ea2876ec32da29b1342e02e7a#eventlog) -> [Reward claimed on BSC](https://bscscan.com/tx/0x58e30595c5bfa3ada0a44e3fd4be89546d88cbab22695081fec27178c18ab29c#eventlog)

First undelegation:\
[Undelegate on BSC](https://bscscan.com/tx/0x1709118184022c18123ce9b27fc7c78d6a9157f19e2ce11e2609b71952fa6e13#eventlog) -> [Undelegate on BC](https://explorer.bnbchain.org/tx/AFE8976DAC8F8ECD1E99FB80EFE951DBEF85717564270C320CE92F93EAB2A87D) -> [Undelegate ACK on BSC](https://bscscan.com/tx/0x1cada1266e390be4f13a453d484e9f9fcdcb062e31139dc3f6552810fcc5c3d6#eventlog) -> [Undelegate claimed on BSC](https://bscscan.com/tx/0x45f64dfa52ce0e8877005a04b966dd19b0b35c7e427a0e3b55b7fa35f585207b#eventlog)

Note: when BNB reserves in the Vault are low, Harvest will trigger an undelegation to top up the reserves.

### Verify reserves on BSC staking system contract

Read contract on BscScan, verify using methods getTotalDelegated, getDelegated:\
[0x0000000000000000000000000000000000002001](https://bscscan.com/address/0x0000000000000000000000000000000000002001#readContract)

For delegator address, use the Vault address: [0x09A18250f99118f40a5D992D537E24b8BD9880F3](https://bscscan.com/address/0x09A18250f99118f40a5D992D537E24b8BD9880F3)

For validator address, convert validator's BC address from [bech32 to hex](https://slowli.github.io/bech32-buffer/).













