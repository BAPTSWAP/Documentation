---
description: >-
  BAPTSWAP allows developers to launch fee-on-transfer supported tokens. Learn
  how here.
---

# Create Your Own Token

<figure><img src=".gitbook/assets/DeployOnBaptSwap.png" alt=""><figcaption></figcaption></figure>

## Deploy Your Token

{% hint style="warning" %}
As of October 2023, **tokens created by other Token Deployer Tools on Aptos, may not be compatible for fee-on-transfer support on Baptswap.**

Note: These tokens can still be traded on Baptswap, but without the possibility to add additional fees, where they operate as normal zero-tax tokens.
{% endhint %}

To have your token tradable with fee-on-swap support on Aptos, Baptswap is the only place where this is possible.

By creating a token through Baptswap, teams can rest assured that their token will work seamless with the Baptswap ecosystem and its unique fee-on-transfer support.

## Creating a Token With the Baptswap Token Deployer

Creating a token on Baptswap is fast and easy. Simply navigate to Baptswap and connect the desired wallet for receiving the Token Admin Rights.&#x20;

On the navigation bar, you can find its Token Deployer Tool.

To create your token, you will have to decide on a few parameters for your token's information:

* Name of the Token (Eg. Moon Coin)
* Symbol (Eg. MOON)
* Total Supply (Eg. 1000000)
* Decimals (Standard for most coins is 8)
* Monitor Supply (If unsure, leave this on true)

Once the token's information is decided, the next step is to execute two transactions with your wallet:

1. Create module for initializing the token.
2. Publish/Deploy token.

The user will have to pay a small network fee for executing a transaction on Aptos, and a Protocol fee of 1 APT.

Congrats, you have now created your own token! To find more information about the token, and to set the token's fees, navigate to the Token Admin Panel.

{% hint style="success" %}
For information on how to create a token on Aptos directly through code without the Token Deployer, [click here](https://aptos.dev/tutorials/your-first-coin/).
{% endhint %}

## Add Liquidity on Baptswap

To become tradable on the DEX, the token listed will need to have LP added to the token through Baptswap's router. This is done through the Liquidity page.

**Important to note:** As soon as liquidity is added, the token is live for being traded on Baptswap.

## Enjoy Your New Environment!

Now that your token is live for trading on Baptswap, where both you and your holders can enjoy a whole new experience, with fee-on-transfer support, never seen before on Aptos!

{% hint style="info" %}
Tokens with LP on multiple exchanges will only have tax supported on Baptswap, meaning that the tokens will still be zero fee tokens on the other DEXes.

By doing this, it can reduce the amount of fees your team can collect from the token's trading volume.
{% endhint %}

## Need Help to List Your Token?

Need help to launch or migrate to Baptswap? Reach out here 👉

Reach out on [Twitter](https://x.com/baptswap) or [Telegram](https://t.me/baptswap).
