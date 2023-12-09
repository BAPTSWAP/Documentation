# 🚀 Token Deployer Tool

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

## Introduction

Launching tokens on the Aptos blockchain is now accessible to everyone, thanks to Baptswap's Token Deployer Tool. This tool is designed for ease of use, requiring no coding knowledge, making it ideal for teams unfamiliar with the technical complexities of blockchain development.

## Understanding Move

In MOVE, the code data is stored under the code module under the resource account.&#x20;

For [contract upgrades](https://aptos.dev/guides/move-guides/upgrading-move-code/), MOVE execute the upgrade logic in system module `code.move` where the upgrade policy and compatibility is checked before the code deployment. After compatibility check, the code written in the resource is replaced through a native function call and will execute the new logic.

### Implications of MOVE's Model

#### **Ownership Control**

The original deployer retains upgrade privileges indefinitely.

#### **Immutability of Ownership**

The owner of the code is fixed post-deployment, making the deployer address the permanent owner.

#### **Token Ownership on Aptos**

Contrary to Solidity, token ownership on Aptos is determined by the wallet holding the owner modules, which cannot be transferred post-deployment.

***

## Baptswap Follows The Owners

Baptswap’s fee-on-transfer support is designed to allocate administrative rights to the token's owner wallet, enabling them to set and modify fees.

### Challenges with Other Deployers

Other deployment tools on Aptos may retain ownership modules within their smart contracts, limiting the actual token owners' control.

***

## Baptswap's Solution

Baptswap's Token Deployer Tool ensures that ownership modules are transferred to the deploying team’s wallet, granting them complete control over their token.

Tokens created with this tool are fully compatible with Baptswap's ecosystem, including its fee-on-transfer features.&#x20;

Alternatively, tokens can be published directly from a wallet owned by the team.

## Compatibility Note

{% hint style="info" %}
As of October 2023, tokens created using other deployer tools on Aptos might not be compatible with Baptswap’s fee-on-transfer support, though they can still be traded as standard zero-tax tokens.

Learn how to create your own token using the Baptswap Token Deployer Tool [here](../../create-your-own-token.md).
{% endhint %}

##

##

## Creating Tokens on Aptos Made Simple

Our goal is to allow everyone to easily deploy and launch tokens on Aptos. Due to Aptos operating a bit different than EVM blockchains, getting started requires some more technical knowledge, than most are used to from networks like Ethereum and Binance Smart Chain. We have therefore created a tool that requires **zero coding knowledge**, to let teams launching their own token!

Learn more about Baptswap's Token Deployer Tool here.

## Understanding the Token Framework on Aptos

In MOVE, the code data is stored under the code module under the resource account.&#x20;

For [contract upgrades](https://aptos.dev/guides/move-guides/upgrading-move-code/), MOVE execute the upgrade logic in system module `code.move` where the upgrade policy and compatibility is checked before the code deployment. After compatibility check, the code written in the resource is replaced through a native function call and will execute the new logic.

There are several implications from the MOVE code storage model:

1. According to contract upgrade policy, the owner of the code has the full control of the upgrade permission.
2. The owner of the code is immutable after the initial deployment.
3. Thus the deployer address own the upgrade privilege forever after the deployment.

Different from Solidity, the ownership of a token on Aptos, is decided by which wallet is holding the owner modules. These modules are set to the wallet publishing a token's module, and can not be transfered to another wallet.

## Baptswap Follows the Tokens Owners

To ensure Baptswap to work in the most efficient way for teams, the fee-on-transfer support allocates the admin rights of a token to the its owner wallet. Only the Token Admin wallet can set, change and claim fees for their individual token.

### Issues With Using Other Token Deployers

Typically when creating tokens with tools provided by other protocols on Aptos, the ownership modules are held back within the smart contracts of the deployers themselves. Tokens are sent to the wallet interacting with the deployers, however they will not receive the full ownership of their token.

### Baptswap's Solution

With Baptswap's Token Deployer, the owner modules are sent to the team's wallet upon token creation, allowing them to claim 100% of the token's ownership for further scaling.

By creating a token through the Baptswap Token Deployer, teams can rest assured that their token will work seamless with the Baptswap ecosystem and its unique fee-on-transfer support.

To make it clear, Baptswap only allows the wallet containing the owner module to add fee-on-transfer support for their token. Therefore the only two ways to get fee-on-transfer support for a token, one of the two requirements below must be met:

* The token is created through Baptswap's own Token Deployer Tool, resulting in the token's modules are published from the team's wallet interacting with the deployer.
* The token is published directly from a wallet owned by the team, resulting that the team controls a wallet with the token's modules.

{% hint style="warning" %}
As of October 2023, **tokens created by other Token Deployer Tools on Aptos, may not be compatible for fee-on-transfer support on Baptswap.**

Note: These tokens can still be traded on Baptswap, but without the possibility to add additional fees, where they operate as normal zero-tax tokens.

[Learn how to create your own token here.](../../create-your-own-token.md)
{% endhint %}
