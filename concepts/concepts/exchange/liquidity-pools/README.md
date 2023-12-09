---
description: How LP providing works
---

# Liquidity Pools

<figure><img src="../../../../.gitbook/assets/LiqPools.png" alt=""><figcaption></figcaption></figure>

## Introduction

Liquidity pools are essential components of the Baptswap platform, allowing users to provide liquidity and earn rewards. This document explains the mechanics of Liquidity Pools and the associated benefits and risks.

## LP Tokens (Liquidity Provider Tokens)

### Definition and Function

LP tokens are issued to users who deposit assets into liquidity pools. They serve as a receipt, representing the user's share in the pool and entitling them to a portion of the trading fees generated.

### Example

> If you deposit BAPT and APT into a pool, you receive BAPT-APT LP tokens, which represent your share in the BAPT-APT Liquidity Pool. These tokens can be redeemed to withdraw your original stake and earned interest.

## Earning from Trading Fees

### How it Works

As a liquidity provider, you earn a portion of the trading fees generated from your pool.

In Baptswap, a 0.90% trading fee is charged on swaps, with 0.30% of that fee added to the liquidity pool involved in the trade.

### Example

> Consider a pool with 10 LP tokens representing 10 BAPT and 10 APT each.
>
> * A trade occurs, and the pool's assets grow to 10.030 BAPT and 10.030 APT.
> * Each LP token's value increases correspondingly.

## Enhanced Earnings on Baptswap

### Unique Fee-on-Transfer Mechanism

Baptswap allows tokens to implement LP Fees up to 15% of their trading volume, which is distributed among liquidity providers in addition to the standard 0.3% swap fee.

This can significantly increase the potential rewards for providing liquidity on Baptswap compared to other exchanges.

{% hint style="success" %}
Compared to other AMMs on Aptos, providing liquidity on Baptswap can be up to 151.5 times more benefitial for providers
{% endhint %}

## Benefits of Providing Liquidity

### Importance for the Exchange

Liquidity is vital for enabling asset swaps on Baptswap. Insufficient liquidity can make swaps difficult, expensive, or impossible.

By providing liquidity, you facilitate trading and earn rewards from trading fees and potentially from Fee-on-Transfer taxes, if applicable.

### Stability and Sustainability

A robust liquidity pool enhances asset stability and mitigates price impact during trading.

### Earnings Sources for LP Providers

LP providers earn from:

* The 0.3% trading fee from each pair trade.
* Additional allocations from Fee-on-Transfer taxes, if implemented on the traded tokens.

### Impermanent Loss

{% hint style="danger" %}
Providing liquidity comes with the risk of impermanent loss, which occurs when the price of your deposited assets changes compared to when you deposited them. This is an important consideration for all potential liquidity providers.
{% endhint %}

\
[“Simply put, impermanent loss is the difference between holding tokens in an AMM and holding them in your wallet.” - Nate Hindman](https://blog.bancor.network/beginners-guide-to-getting-rekt-by-impermanent-loss-7c9510cb2f22)
