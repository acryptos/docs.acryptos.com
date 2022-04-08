# Liquidizer Vaults

Liquidizer Vaults are designed to automate yield farming on top of illiquid farms and "liquidize" them.

Parameters of Liquidizer Vaults are:

* Reserves: The amount of liquid reserves in the Vault that are not locked in the underlying protocol and available for users to withdraw.
* Reserve Ratio: The ratio of liquid reserves in the Vault as a percentage of the total Vault TVL.
* Target Reserve Ratio: The Reserve Ratio the Vault aims to maintain.
* Amp: The [StableSwap](https://curve.fi/files/stableswap-paper.pdf) parameter the Vault uses to calculate withdrawal "slippage".

When a user withdraws:

* Any amount that does not bring Reserves below Target Reserves is withdrawn as normal.
* Any amount that brings Reserves below Target Reserves experiences "slippage" as if they were trading against a StableSwap pool with 2 balances: Reserves and Target Reserves.

For example, if a user were to withdraw 100 FTM from a Vault with Reserves of 1000 FTM and a Target Reserve of 2000 FTM, it would be as if he was selling 100 FTMA to a StablePool with 2000 FTMA and 1000 FTMB.



