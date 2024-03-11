# Create Your Own Token

<figure><img src=".gitbook/assets/DeployOnBaptSwap.png" alt=""><figcaption></figcaption></figure>

## Introduction

Baptswap offers a unique zero-code tool to launch tokens with fee-on-transfer support. This guide provides a step-by-step process for token deployment on Baptswap.

## Deploying Your Token

{% hint style="warning" %}
As of October 2023, it's important to note that **tokens deployed using other Token Deployer Tools on the Aptos** blockchain **may not be compatible with** Baptswap's **fee-on-transfer feature**.&#x20;

These tokens **can still be traded on Baptswap**, but they will function as standard tokens **without additional fee capabilities**.
{% endhint %}

## Advantages of Using Baptswap

Deploying your token through Baptswap ensures seamless integration with the Baptswap ecosystem, including its unique fee-on-transfer functionality. This is an exclusive feature available only on Baptswap for tokens on the Aptos blockchain.

## Steps to Create a Token

Creating a token on Baptswap is fast and easy. Simply navigate to Baptswap and connect the desired wallet for receiving the Token Admin Rights.&#x20;

### **Token Information**

Start by connecting your wallet to Baptswap and accessing the Token Deployer Tool. You'll need to define key parameters for your token:

* Name (e.g., Moon Coin)
* Symbol (e.g., MOON)
* Total Supply (e.g., 1 000 000)
* Decimals (Standard is 8)

<figure><img src=".gitbook/assets/Screenshot 2024-03-11 at 12.45.06.png" alt=""><figcaption></figcaption></figure>

### **Token Deployment**

Wait for the token to be compiled and execute transaction.

* Create a module for initializing the token.
* Publish/Deploy the token.
* Note: There will be a nominal network fee on Aptos and a Protocol fee of 1 APT.

Once the token is successfully created, a pop-up window appears. Here you can quickly copy the contract address. There is also a button that redirects to the admin dashboard for managing fees.

<figure><img src=".gitbook/assets/Screenshot 2024-03-11 at 12.45.58.png" alt=""><figcaption></figcaption></figure>

### **Admin Dashboard**

Congrats, you have now created your own token! To find more information about the token, and to set the token's fees, navigate to the Token Admin Dashboard through the pop-up screen, or paste your token's address to the URL like this link:

> https://baptswap.com/#/admin-token/your\_tokens\_address\_here

### Adding Fees

{% hint style="success" %}
**We recommend you to initialize and save the fees before adding any liquidity to the token.**

All individual liquidity pairs created before fees have been initialized, have to be manually enabled from the "My Active Pairs" page in the Admin Dashboard.

All pairs created after fees are initialized will automatically adopt the fees settings.
{% endhint %}

For adding fees to your token, navigate to the admin dashboard. To enable fees for the token, press the "Initialize Fee on Transfer" button, type in the desired fees for each option, then press the save button appearing. After confirming the transaction, all pairs created from now will adopt the fee settings.

<figure><img src=".gitbook/assets/Screenshot 2024-03-11 at 12.46.12.png" alt=""><figcaption></figcaption></figure>

## Adding Liquidity on Baptswap

To enable trading on the DEX, add liquidity to your token through [Baptswap's Pool page](https://baptswap.com/#/pools/v2).

Once liquidity is added, your token becomes available for trading on Baptswap.

## Enjoy Your New Environment!

Your token is now live on Baptswap, featuring fee-on-transfer support — a first on the Aptos blockchain!

{% hint style="info" %}
Note that tokens with LP on multiple exchanges will only support fee-on-transfer on Baptswap.

By adding LP on other exchanges, it can reduce the amount of fees your team can collect from the token's trading volume.
{% endhint %}

## Upload Logo to wallets and Baptswap

For uploading the logo of your token so it natively displays on Aptos wallets and on Baptswap, follow this [guide](https://github.com/hippospace/aptos-coin-list/tree/main).

## Support and Assistance

Need help with launching or migrating your token to Baptswap? Connect with us on [Twitter](https://x.com/Baptswap) or [Telegram](https://t.me/baptlabs) for assistance.

{% hint style="success" %}
For developers wishing to deploy directly via code without using the Token Deployer, [click here](https://aptos.dev/tutorials/your-first-coin/).
{% endhint %}
