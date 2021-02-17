# Security & Risks

## RISK WARNING

This project is in beta. Use at your own risk.

### ACryptoS Dev Team Access

* **ACryptoS Dev Team can control all assets in Vaults behind a 48 hour timelock.**
* **ACryptoS Dev Team can mint ACS token behind a 48 hour timelock.**
* **ACryptoS Dev Team can mint ACSI token behind a 48 hour timelock.**
* **ACryptoS Dev Team can control all reward parameters of ACS Farms behind a 6 hour timelock.**
* **ACryptoS Dev Team can control all reward parameters of ACSI Farms behind a 6 hour timelock.**
* **ACryptoS Dev Team can control all fee parameters of StableSwap behind a 72 hour timelock. ACryptoS Dev Team can control destination of StableSwap admin fees.**
* ACryptoS Dev Team cannot control assets in Farms.
* ACryptoS Dev Team cannot control assets in StableSwap.

### Other Risks

* Smart contract risks, both ACryptoS contracts and third parties our Vaults interact with.
* Risks in underlying assets and smart contracts.
* "Impermanent loss" risk.
* Risk of StableSwap assets losing their pegs.

### APRs/Returns

APRs/returns shown on the UI include the performance and the workers fees, but **do not include** the other fees \(withdrawal, harvest\), which will result in a negative return if you enter and exit a position quickly.

High returns/APRs almost certainly mean a high risk. The calculated APR/return depends on the underlying value of the token in the vault and the token\(s\) being farmed, including ACS and ACSI, which can be very volatile and/or inflationary.

## Smart Contracts

### Audit

**The project has been audited by** [**DefiYield**](https://defiyield.info/audits)**.**

**Check the** [**full audit report here**](https://defiyield.info/assets/pdf/ACryptoS.pdf)**.**

Smart contracts are forked from yearn.finance \(Vault, Controller, Strategy\), SushiSwap \(MasterChef\), Uniswap \(Uni\), Curve \(StableSwap\).

### Deployed

All deployed contracts have [verified and published source codes on BscScan](https://app.acryptos.com/contracts/).

