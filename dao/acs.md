# $ACS Token

## Liquidity

Uniswap V3 (BSC): [Trade](https://app.1inch.io/#/56/advanced/swap/BNB/0x8888888888f004100C0353d657BE6300587A6CcD) / [Liquidity](https://app.uniswap.org/add/0x8888888888f004100C0353d657BE6300587A6CcD/ETH/10000?chain=bnb) Info: [US](https://app.uniswap.org/explore/pools/bnb/0x86D708404d0DB1D97843E66D4Ed6B86d11bE705B) / [DS](https://dexscreener.com/bsc/0x86D708404d0DB1D97843E66D4Ed6B86d11bE705B)\
Equilibre (Kava): [Trade](https://equilibrefinance.com/swap) / [Liquidity](https://app.acryptos.com/vaults/2222/0x05Aa420a97449c0C54B369BAfaA9Ca43a77004eD/) Info: [DS](https://dexscreener.com/kava/0x395e6e5f3df5120fda26be1849d4388cc2500435)

Bridge ACS: [https://app.acryptos.com/acs/bridge/](https://app.acryptos.com/acs/bridge/)\
Migrate ACS: [https://app.acryptos.com/acs/migrate/](https://app.acryptos.com/acs/migrate/)

[Dex Screener Watchlist](https://dexscreener.com/watchlist/9qDR83Yk0EjRCCPE26sH)

## Multichain.org Incident - July 2023

The Multichain.org bridge stopped working on 7 July 2023 following abnormal movements of locked assets. \~170K of bridged ACS was stuck and under the control of unknown entities. An announcement was made to ask users to remove ACS paired liquidity as a migration plan was being worked on. A governance vote was taken to [approve the migration](https://vote.acryptos.com/#/proposal/0x16b1bcf3b151f9de38b151616f5d83bfdc2415a677cd5953ec1be2d0343009e1).

A new ACS token is deployed at 0x8888888888f004100C0353d657BE6300587A6CcD across several chains.

The new token was designed with certain features to mitigate bridging risks:

* Bridging is achieved by passing cross chain messages. This is using Layer Zero initially, and can be upgraded to use any combination of protocols.
* ACryptoS Dev team controls new token contracts including the ability to pause and blacklist in the event of bridge / messaging protocol exploit.
* Bridged balances are reconciled on the canonical chain (BSC). Bridging can only be done to/from the canonical chain, and will fail if they cannot be reconciled (i.e. more balance bridged in than has been bridged out).

There is a migration feature which will allow users to migrate 1:1 the old/Multichain.org ACS tokens. Migration will be paused if the contract detects abnormal changes in the locked Multichain.org ACS tokens.

Withdraw from ACS vault with no penalty fees: [https://app-legacy.acryptos.com/core/](https://app-legacy.acryptos.com/core/)

## ACS and ACSI Token Merger

There were discussions on simplifying ACryptoS tokenomics to a single token, and a [governance vote was passed](https://vote.acryptos.com/#/proposal/0xe9b6e77cfeafaf95556ed7e7d882d2792c0eaca32c317688f56cf7b037521de4) to merge ACSI at a 4:1 ratio to the new ACS token.

Withdraw from ACSI vault with no penalty fees: [https://app-legacy.acryptos.com/core/](https://app-legacy.acryptos.com/core/)\
ACSI migration to ACS token: [https://app.acryptos.com/acs/migrate/](https://app.acryptos.com/acs/migrate/)

