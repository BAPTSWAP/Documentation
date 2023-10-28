# Fees

### Liquidity provider fees[​](https://docs.uniswap.org/contracts/v2/concepts/advanced-topics/fees#liquidity-provider-fees) <a href="#liquidity-provider-fees" id="liquidity-provider-fees"></a>

There is a **0.9%** fee for swapping tokens. **This fee is split by liquidity providers proportional to their contribution to liquidity reserves, but also allocating a part to the Baptswap Treasury through the Protocol Fee.**

Swapping fees are immediately deposited into liquidity reserves. This increases the value of liquidity tokens, functioning as a payout to all liquidity providers proportional to their share of the pool. Fees are collected by burning liquidity tokens to remove a proportional share of the underlying reserves.

Since fees are added to liquidity pools, the invariant increases at the end of every trade. Within a single transaction, the invariant represents `token0_pool / token1_pool` at the end of the previous transaction.

There are many community-developed tools to determine returns. You can also read more in the docs about how to think about [LP returns](https://docs.uniswap.org/contracts/v2/concepts/advanced-topics/understanding-returns).

### Protocol Fees[​](https://docs.uniswap.org/contracts/v2/concepts/advanced-topics/fees#protocol-fees) <a href="#protocol-fees" id="protocol-fees"></a>

At the moment there is a 0.60% Protocol Fee . However, it is possible for the fees to be turned off or reduced in the future.

More information about a potential future protocol fee can be found here (blog post coming soon).

### Protocol Charge Calculation[​](https://docs.uniswap.org/contracts/v2/concepts/advanced-topics/fees#protocol-charge-calculation) <a href="#protocol-charge-calculation" id="protocol-charge-calculation"></a>

The Protocol Fees do not not affect the fee paid by traders, but would affect the amount received by liquidity providers.

Rather than calculating this charge on swaps, which would significantly increase gas costs for all users, the charge is instead calculated when liquidity is added or removed.
