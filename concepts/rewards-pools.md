# Rewards Pools

{% hint style="warning" %}
This page requires the reader to be familiar with the Fee-on-Transfer concept. Before reading, make sure to check out the [Fee-on-Transfer introduction](../fee-on-transfer/).

_Diclaimer: The Protocol is not able to impact the performance of a Reward Pool. The return of a Reward Pool is decided by external factors outside the control of the Baptswap Protocol_
{% endhint %}

All tokens with Reward Fees enabled through Baptswap's Fee-on-Transfer support, offer volume based Reward Pools through the Earn page. Here holders have the options to stake their holdings to increase their positions.

For each pair including a token with Reward Fees, a Reward Pool is created. A token can potentially have multiple different Reward Pools, based on the amount of pairs tied to the token.&#x20;

The amount of Reward Fees set to a specific token, will follow all pairs including that token. However, each Reward Pool will only build up rewards for stakers from the specific pair tied to the pool.

> **Example 1:**
>
> BAPT has x% Reward Fees.
>
> Both the BAPT-APT and BAPT-USDC pairs exists.
>
> A Reward Pool for BAPT/APT is created, and a Reward Pool for BAPT/USDC is created.
>
> Users can freely choose the amount of tokens to deposit into each pool.

> **Scenario 1, Given Example 1:**
>
> Alice swaps APT into BAPT.
>
> BAPT's Reward Fees are collected in the output token (here: BAPT), and sent to the BAPT-APT Rewards Pool.

> **Scenario 2, Given Example 1:**
>
> Alice swaps BAPT into USDC.
>
> BAPT's Reward Fees are collected in the output token (here: USDC), and sent to the BAPT-USDC Reward Pool.

### Pool Performance

_**The Baptswap Protocol can not impact the perfomance of any Reward Pool.** The Earn Page is simply for external teams to add an additional feature for their token trading on Baptswap._

The performance of a specific Reward Pool depends on the following factors:

1. The pair's trading volume.
2. The amount of Fees (%) allocated to Reward Fees.
3. The amount of tokens staked in the Reward Pool.

Rewards are accumulated based on a holder's size of the pool. The bigger portion of the tokens a holder is staking, compared to the total staked amount in the pool, the higher rewards can be claimed by the holder.

### Dual Reward System

Each Reward Pool will accumulate both assets in the pair it is tied to. The result of this, is that holders who stake their tokens, will claim both the native staked token, and the opposite token in the pair.

The ratio between the rewards accumulated will depend on the pair's trading volume each direction of the swap. If a pair has more trading volume from X to Y, holders will receive a higher amount of rewards in Y compared to X.

> Example 2:
>
> Alice deposits BAPT into the BAPT-APT pool.
>
> When claiming rewards, Alice receives rewards in both BAPT and APT.
>
> If the trading volume is higher for swap from APT to BAPT, than from BAPT to APT, Alice will receive a higher reward in BAPT.

### Case 1: One Token in a Pair With Rewards&#x20;

> A pair is created between BAPT and APT.
>
> BAPT has x% Reward Fees enabled. Aptos does not have Reward Fees.
>
> A Reward Pool BAPT-APT is created, and users can deposit BAPT to earn.

### Case 2: Both Tokens in Pair With Rewards

> A pair is created between BAPT and MOON.
>
> BAPT has 2% Reward Fees enabled. MOON has 4% Reward Fees enabled.
>
> A Reward Pool BAPT-MOON is created, and users can deposit BAPT to earn.
>
> A Reward Pool MOON-BAPT is created, and users can deposit MOON to earn.
>
>
>
> For each swap, 6% Reward Fees are extracted from the transaction and distributed between both Reward Pools.&#x20;
>
> 33.3% of the Fees are sent to the BAPT-MOON pool for BAPT holders.
>
> 66.7% of the Fees are sent to the MOON-BAPT pool for MOON holders.
