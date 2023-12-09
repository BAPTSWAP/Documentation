# 🥩 Reward Pools

{% hint style="warning" %}
This document assumes familiarity with the Fee-on-Transfer concept. For a foundational understanding, please refer to the [Fee-on-Transfer Introduction](fee-on-transfer/) section before proceeding.
{% endhint %}

## Disclaimer

_The Protocol is not able to impact the performance of a Reward Pool. The return of a Reward Pool is decided by external factors outside the control of the Baptswap Protocol._

## Overview

Baptswap facilitates Reward Pools for all tokens that enable Reward Fees via its Fee-on-Transfer feature. On the Earn page, token holders can stake their assets to augment their holdings.

## Creation of Reward Pools

A unique Reward Pool is established for each pair involving a token with Reward Fees. Thus, a single token may be associated with multiple Reward Pools corresponding to its different trading pairs. The set Reward Fees for a token apply across all its pairs, but each Reward Pool accrues rewards only from its specific pair.

## Examples

> **Example 1:**
>
> If BAPT has x% Reward Fees and is part of BAPT-APT and BAPT-USDC pairs, separate Reward Pools for BAPT/APT and BAPT/USDC will be established.
>
> Users can decide how many tokens to contribute to each pool.

> **Scenario 1, Given Example 1:**
>
> If Alice swaps APT for BAPT, the Reward Fees in BAPT are directed to the BAPT-APT Reward Pool.

> **Scenario 2, Given Example 1:**
>
> If Alice exchanges BAPT for USDC, the Reward Fees in USDC are allocated to the BAPT-USDC Reward Pool.

## Pool Performance Factors

The performance of a specific Reward Pool depends on the following factors:

1. The trading volume of the pair.
2. The percentage of fees allocated to Reward Fees.
3. The total amount of tokens staked in the Reward Pool.

The stakers' rewards are proportional to their share in the pool; a larger stake equates to higher potential rewards.

## Dual Reward System

Each Reward Pool accumulates both assets from its associated pair. Stakers can claim rewards in both the staked token and its pair counterpart. The reward ratio is influenced by the trading volumes in each swap direction.

> Example 2:
>
> If Alice stakes BAPT in the BAPT-APT pool, she will receive rewards in both BAPT and APT. The dominant trading direction determines the higher reward component.

## Case 1: One Token in a Pair With Rewards&#x20;

> For a BAPT-APT pair where only BAPT has Reward Fees, a BAPT-APT Reward Pool is created for BAPT deposits.

## Case 2: Both Tokens in Pair With Rewards

> In a BAPT-MOON pair with both tokens having Reward Fees (2% for BAPT, 4% for MOON), separate Reward Pools for BAPT-MOON (deposit BAPT) and MOON-BAPT (deposit MOON) are established.
>
> For each swap, 6% Reward Fees are distributed between both pools: 33.3% to BAPT-MOON and 66.7% to MOON-BAPT.
