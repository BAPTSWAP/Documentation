# Understanding Returns

## Introduction

This guide provides an insight into how liquidity providers earn returns and the associated risks in the Baptswap ecosystem.

## Liquidity Provider Incentives

### Fee Rewards

Liquidity providers are rewarded with a portion of the fees generated from trading within their pools. Baptswap charges a 0.9% fee for swapping tokens, distributed among liquidity providers and the Baptswap Treasury.

### Token Distribution

Providers receive “liquidity tokens” proportional to their share in the liquidity pool. These tokens represent a claim on the pool's assets and are not meant for trading.

## Risks and Returns

### Understanding Risks

Market making, while potentially profitable, carries the risk of losses, especially during significant price movements of the underlying assets. An in-depth analysis of these risks is available in [this article](https://medium.com/@pintail/uniswap-a-good-deal-for-liquidity-providers-104c0b6816f2).

### Example Scenario

The article provides an example where a provider's stake in a pool could lead to missed profits compared to simply holding the assets due to market price changes. This scenario illustrates the concept of "impermanent loss".

## Impermanent Loss Explained

### Definition

Impermanent loss occurs when the price of assets in a liquidity pool changes compared to when they were deposited. The loss is 'impermanent' as it can be reversed if the prices return to their original state.

### Calculation

The loss can be calculated using the formula:&#x20;

`impermanent_loss = 2 × price_ratio / (1+price_ratio) − 1impermanent_loss = 2 × price_ratio​ / (1+price_ratio) − 1`

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

### Impact at Different Price Ratios

For example:

* A 1.25x price change results in a 0.6% loss relative to holding (HODL).
* A 2x price change results in a 5.7% loss relative to HODL.
* Larger price changes result in increasingly significant losses.

### Direction of Price Change

The direction of the price change (increase or decrease) does not affect the magnitude of the impermanent loss.

## Conclusion

While providing liquidity on Baptswap can be rewarding due to trading fees, it is important for liquidity providers to be aware of the risks, particularly impermanent loss. Understanding these dynamics is crucial for making informed decisions in the decentralized finance landscape.
