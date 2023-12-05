---
description: Graphics are referenced from Uniswap.
---

# How Baptswap Works

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption><p>Graphics are referenced from Uniswap.</p></figcaption></figure>

Baptswap is an _automated liquidity protocol_ powered by a constant product formula and implemented in a system of smart contracts on the Aptos blockchain. It obviates the need for trusted intermediaries, prioritizing **decentralization**, **censorship resistance**, and **security**. Baptswap is **open-source software.**

Each Baptswap smart contract, or pair, manages a liquidity pool made up of reserves of two tokens.

Anyone can become a liquidity provider (LP) for a pool by depositing an equivalent value of each underlying token in return for pool tokens. These tokens track pro-rata LP shares of the total reserves, and can be redeemed for the underlying assets at any time.

![Graphics are referenced from Uniswap.](https://docs.uniswap.org/assets/images/lp-c0b1b03ef921f1325971fa8ab6e9a4f1.jpg)

Pairs act as automated market makers, standing ready to accept one token for the other as long as the “constant product” formula is preserved. This formula, most simply expressed as `x * y = k`, states that trades must not change the product (`k`) of a pair’s reserve balances (`x` and `y`). Because `k` remains unchanged from the reference frame of a trade, it is often referred to as the invariant. This formula has the desirable property that larger trades (relative to reserves) execute at exponentially worse rates than smaller ones.

In practice, Baptswap by default applies a 0.90% fee to trades, where 0.30% is added to reserves. As a result, each trade actually increases `k`. This functions as a payout to LPs, which is realized when they burn their pool tokens to withdraw their portion of total reserves. In the future, this fee may be reduced, with the remaining being withheld as a protocol-wide charge.

![Graphics are referenced from Uniswap.](https://docs.uniswap.org/assets/images/trade-b19a05be2c43a62708ab498766dc6d13.jpg)

Because the relative price of the two pair assets can only be changed through trading, divergences between the Baptswap price and external prices create arbitrage opportunities. This mechanism ensures that Baptswap prices always trend toward the market-clearing price.

## Further reading

To see how token swaps work in practice, and to walk through the lifecycle of a swap, check out [Swaps](../core-concepts/swaps.md). Or, to see how liquidity pools work, see [Pools](../core-concepts/pools.md).

Ultimately, of course, the Baptswap Protocol is just smart contract code running on the Aptos Network. To understand how they work, head over to [Smart Contracts](../technical-reference/smart-contracts/).
