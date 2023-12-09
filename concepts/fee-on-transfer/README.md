---
description: Scale your project like never before on Aptos.
---

# 💸 Fee-on-Transfer

{% hint style="warning" %}
This page requires the reader to be familiar with what Fee-on-Transfer support is. Before reading, make sure to check out [this glossary page](fee-on-transfer-glossary.md).

As of October 2023, **tokens created by other Token Deployer Tools on Aptos,** **are not compatible for fee-on-transfer suppor**t on Baptswap.

Note: These tokens can still be traded on Baptswap, but without the possibility to add additional fees, where they operate as normal zero-tax tokens.

[Learn how to create your own token here.](../../create-your-own-token.md)
{% endhint %}

## **Token Fee Structure in Baptswap**

In Baptswap, the fee dynamics are intricately linked with individual tokens and allow for a high degree of flexibility, offering token teams control over their financial structure. Here's a detailed explanation of how the fees are structured and distributed within the platform:

### Token-Based Fee Mechanism:

1. **Individualized Fee Control**: The fees are attached to each specific token. The responsibility for setting these fees lies with the token's owner wallet, which is the wallet address that houses the token's modules.
2. **Universal Application**: When a token has its fee mechanism activated, every trading pair containing this token will adhere to and collect the fees as predefined.

### Customizable Fee Distribution:

Token teams have the liberty to customize their fee distribution, tailoring it to fit their strategic objectives. The fees can be routed to three primary destinations:

1. **Team Fees**:
   * This portion is directly claimable by the token owner via the Token Admin Panel.
   * Usage: These fees can serve a myriad of purposes, often directed towards operational costs such as marketing initiatives, development efforts, or other project-specific requirements.
2. **Rewards Fees**:
   * Destination: These fees flow automatically to the individual token's unique rewards pool.
   * Benefits: Token holders can leverage this by staking their tokens in the pool. In doing so, they stand to earn rewards based on the token's trading volume.
   * Dual Reward System: Notably, the reward isn't limited to the token alone. When trading occurs between a token pair, say BAPT/APT, stakers receive dividends in both the traded tokens — in this example, both BAPT and APT.
3. **LP (Liquidity Pool) Fees**:
   * This portion is allocated to strengthen the token's liquidity pool.
   * By directing fees to enhance liquidity, token teams can potentially stabilize their token's price, making it less volatile from trading impacts.

### Distribution Flexibility:

Token teams have the liberty to toggle between these fee destinations as per their project's evolving needs. The only stipulation is that the cumulative fee percentage should not exceed 15% each way. Within this threshold, teams can adjust the distribution percentages among the three destinations as they deem fit.

{% hint style="info" %}
The fees are set for buys and sells individually, meaning that the max fees for a team to set for their token is 15%/15%.

However, the team may choose to set the fees different, like for example 0% for buys and 15% for sells.\
\
To ensure teams for not creating honeypots, Baptswap follows these two universal rules for token fees:

\
`(Buy_Team_Fee + Buy_Rewards_Fee + Buy_Auto_LP_Fee <= 15)`\
\
`(Sell_Team_Fee + Sell_Rewards_Fee + Sell_Auto_LP_Fee <= 15)`
{% endhint %}

{% hint style="success" %}
Baptswap provides a comprehensive yet flexible fee structure, empowering token teams to optimize their economic models in a manner that aligns with their project's vision and operational needs.
{% endhint %}
