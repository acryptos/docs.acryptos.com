# ACS

## Multichain.org Incident - July 2023

The Multichain.org bridge stopped working on 7 July 2023 following abnormal movements of locked assets. \~170K of bridged ACS was stuck and under the control of unknown entities. An announcement was made to ask users to remove ACS paired liquidity as a migration plan was being worked on.

A new ACS token is deployed at 0x8888888888f004100C0353d657BE6300587A6CcD on BSC, Kava EVM and Arbitrum.

The new token was designed with certain features to mitigate bridging risks:

* Bridging is achieved by passing cross chain messages. This is using Layer Zero initially, and can be upgraded to use any combination of protocols.
* ACryptoS Dev team controls new token contracts including the ability to pause and blacklist in the event of bridge / messaging protocol exploit.
* Bridged balances are reconciled on the canonical chain (BSC). Bridging can only be done to/from the canonical chain, and will fail if they cannot be reconciled (i.e. more balance bridged in than has been bridged out).

There is a migration feature which will allow users to migrate 1:1 the old/Multichain.org ACS tokens. Migration will be paused if the contract detects abnormal changes in the locked Multichain.org ACS tokens.

