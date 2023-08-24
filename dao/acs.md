# ACS

## Liquidity

Uniswap V3 (BSC): [Trade](https://app.uniswap.org/#/swap?inputCurrency=ETH\&outputCurrency=0x8888888888f004100c0353d657be6300587a6ccd\&chain=bnb) / [Liquidity](https://app.uniswap.org/#/add/0x8888888888f004100C0353d657BE6300587A6CcD/0x09A18250f99118f40a5D992D537E24b8BD9880F3/10000?chain=bnb) Info: [US](https://info.uniswap.org/#/bnb/pools/0xf41e4edd13712be90604c08664d0e02eebb6d794) / [DS](https://dexscreener.com/bsc/0xf41e4edd13712be90604c08664d0e02eebb6d794)\
Equilibre (Kava): [Trade](https://equilibrefinance.com/swap) / [Liquidity](https://app.acryptos.com/vaults/2222/0x05Aa420a97449c0C54B369BAfaA9Ca43a77004eD/) Info: [DS](https://dexscreener.com/kava/0x395e6e5f3df5120fda26be1849d4388cc2500435)\
Chronos (Arbitrum): [Trade](https://app.chronos.exchange/) / [Liquidity](https://app.chronos.exchange/liquidity/0x31440D82F14e36Be8EDE9E47137E3dfFEEf32C51) Info: [DS](https://dexscreener.com/arbitrum/0x31440d82f14e36be8ede9e47137e3dffeef32c51)\
Archly (Base): [Trade](https://www.archly.fi/swap) / [Liquidity](https://www.archly.fi/liquidity/0x6af6C8De5e2cA6C4E9ab156a4652fF242292D6Ff) Info: [DS](https://dexscreener.com/base/0x6af6c8de5e2ca6c4e9ab156a4652ff242292d6ff)

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

