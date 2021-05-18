# Security & Risks

The overriding focus on safety and risk management is what sets ACryptoS apart from most DeFi projects.

In this section the major risks involved with investing funds in DeFi projects will be described along with the steps that ACryptoS have taken to mitigate these.

Be aware that investing in any DeFi project has risk. DeFi is relatively new and black swan events could occur that no-one has predicted. Only invest what you can afford to lose and always do your own research \(DYOR\) before committing funds to any project.

\*\*This project is in beta. Use at your own risk.

Resources:

[Frequently Asked Questions](faq.md)

### ACryptoS Dev Team Access

* **ACryptoS Dev Team can control all assets in Vaults behind a 48 hour timelock.**
* **ACryptoS Dev Team can mint ACS token behind a 48 hour timelock.**
* **ACryptoS Dev Team can mint ACSI token behind a 48 hour timelock.**
* **ACryptoS Dev Team can control all reward parameters of ACS Farms behind a 6 hour timelock.**
* **ACryptoS Dev Team can control all reward parameters of ACSI Farms behind a 6 hour timelock.**
* **ACryptoS Dev Team can control all fee parameters of StableSwap behind a 72 hour timelock. ACryptoS Dev Team can control destination of StableSwap admin fees.**
* ACryptoS Dev Team cannot control assets in Farms.
* ACryptoS Dev Team cannot control assets in StableSwap.

#### Mitigations

Community [timelock monitor](https://unrekt.net/acryptos/timelock.html) and Telegram [timelock monitor bot](https://t.me/acryptos9/59652).

### Other Risks

* Smart contract risks, both ACryptoS contracts and third parties our Vaults interact with.
* Risks in underlying assets and smart contracts.
* "Impermanent loss" risk.
* Risk of StableSwap assets losing their pegs.

### APRs/Returns

APRs/returns shown on the UI include the performance and the workers fees, but **do not include** the other fees \(withdrawal, harvest\), which will result in a negative return if you enter and exit a position quickly.

High returns/APRs almost certainly mean a high risk. The calculated APR/return depends on the underlying value of the token in the vault and the token\(s\) being farmed, including ACS and ACSI, which can be very volatile and/or inflationary.

## Smart Contracts

### Audits

[**Hacken - Complete**](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210331-Hacken-Complete.pdf) **\(31 Mar 2021\)**  
[**Certik - CAKE Vault Strategy**](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210324-Certik-StrategyACryptoSCakeTokenTokenV2.pdf) **-** [**1**](https://www.certik.org/projects/acryptos) **\(24 March 2021\)**  
[**Hacken - ACryptoS Farm V2**](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210218-Hacken-ACryptoSFarmV2.pdf) **-** [**1**](https://hacken.io/wp-content/uploads/2021/02/20210218-Hacken-ACryptoSFarmV2.pdf) **\(18 Feb 2021\)**  
[**DefiYield.info**](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210128-defiyield.info.pdf) **-** [**1**](https://defiyield.info/assets/pdf/ACryptoS.pdf) **\(28 Jan 2021\)**  
Smart contracts are forked from yearn.finance \(Vault, Controller, Strategy\), SushiSwap \(MasterChef\), Uniswap \(Uni\), Curve \(StableSwap\).

### Deployed

All deployed contracts have [verified and published source codes on BscScan](https://app.acryptos.com/contracts/).

