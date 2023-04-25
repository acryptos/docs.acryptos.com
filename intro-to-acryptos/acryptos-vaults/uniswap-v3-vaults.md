# Uniswap V3 Vaults

Uniswap V3 Vaults are our first multi-token vaults.

## Exploit Risk Mitigations

The multi-token nature of the vaults and their auto-rebalancing feature on concentrated liquidity AMMs make them vulnerable to price manipulation/flash loan type attacks. We have implemented some mitigations to address this:

* We use historical TWAP to detect price volatility / manipulation, which pauses Vault functionality.
* There is a cooldown period after every vault rebalance, which pauses Vault functionality.
* Imbalanced deposits are subject to an equilibrium fee (earned by the Vault). This fee applies only to the imbalanced portion of the deposit and will be similar to if the user swapped within the underlying pool to make a balanced deposit.

The risk of attacks increases as Vault TVL forms the bulk of the underlying pool. When this happens, the Vault should be paused, and users should withdraw from the Vault as soon as possible.

