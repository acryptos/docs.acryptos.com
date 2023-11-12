# ACLM (Advanced Concentrated Liquidity Manager)

ACLM (Advanced Concentrated Liquidity Manager/Uniswap V3) Vaults are our first multi-token vaults.

Our Strategy automatically compounds fees and rebalances its position around the current price.&#x20;

This allows our Vault to maintain very tight positions around stable / pegged pools (e.g. 1-tick / 0.01% range on USDC/USDT), and wider rages on more volatile pools.

Do note that the effects of impermanent loss can be much more pronounced on concentrated liquidity AMMs like Uniswap V3.

## Exploit Risk Mitigations

The multi-token nature of the vaults and their auto-rebalancing feature on concentrated liquidity AMMs make them vulnerable to price manipulation/flash loan type attacks. We have implemented some mitigations to address this:

* We use historical TWAP to detect price volatility / manipulation, which pauses Vault functionality.
* There is a cooldown period after every vault rebalance, which pauses Vault functionality.
* Deposits and withdrawals are subject to slippage checks. Users should check and confirm the correct amounts to be received on the UI before signing transactions.

The risk of attacks increases as Vault TVL forms the bulk of the underlying pool.

