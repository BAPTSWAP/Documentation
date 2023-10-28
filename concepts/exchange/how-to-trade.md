# How to Trade



<figure><img src="../../.gitbook/assets/HowToTrade.png" alt=""><figcaption></figcaption></figure>

Trading on Baptswap is very easy compared to most exchanges. You aren't going to be overwhelmed by charts or jargon, and calculations are all handled for you.

### Getting set up to trade

Before you can trade, you will need a Aptos-compatible wallet. You can learn how to get one [here](broken-reference). You will also need to have some APT tokens to trade with. You can learn how to get some [here](broken-reference).

### Trading on the BAPTSWAP exchange

1\. Go to the exchange page [here](https://baptswap.com/swap).

2\. Unlock your Aptos-compatible wallet by clicking **Unlock Wallet** (you can also **Connect** in the top right-hand corner). If you haven't yet connected your wallet to BAPTSWAP, you can view the guide to [here](broken-reference).

3\. Choose the token you want to trade from the dropdown menu in the "From" section. The default setting is APT.

Whichever token you choose, you will need to make sure you have some to trade with. Your balance is shown above the token dropdown menu.

4\. Choose the token you want to trade to in the "To" section as above. Next, type an amount for your "To" currency by clicking inside the input box.

Your "From" currency amount will be estimated automatically. You can also type your "From" amount and have the "To" amount estimate automatically if you like.

5\. Check the details, and click the **Swap** button.

6\. A window with more details will appear. Check the details are correct.

When you are ready, click the **Confirm Swap** button. Your wallet will ask you to confirm the action.

7\. Done! You can click **View on the Aptos Explorer** to see your transaction details on the explorer.

## How come my transaction won't go through?

BAPTSWAP is a DeFi application such that it interacts with the wallet to complete on-chain transactions for swapping, creating LPs, staking in farms and pools, etc. &#x20;

### Gas Fees

As such, the first thing is to **make sure you have enough APT to pay for the gas fee** of the on-chain transactions. Typically, gas fee fluctuates depending on the number of transactions in the queue, if there are more transactions, a higher gas fee may be required to push through the transaction. On Aptos chain, the gas fee typically ranges from cents to a dollar USD in APT. Learn more about [gas fee here](https://aptos.dev/concepts/gas-txn-fee/).&#x20;

### Transaction Fees

If your swapping action still doesn't go through and it is displaying an error for you to revise the slippage -- you may want to check if the tokens you are trying to swap has **any fees and restrictions on transactions**.

It is not uncommon for tokens on BAPTSWAP to include a **transaction fee** in their contracts, usually these fees could be used for funding a treasury or towards rewarding holders for staking the token -- for example, BAPT[ has an 8% tax on every transaction](https://baptlabs.com) for sending to the treasury address, rewarding stakers and supporting the LP.&#x20;

With the transaction fee, whether it is inclusive (a portion of the swap amount is sent elsewhere than your address so the output is less than expected for the estimated input) or exclusive (requiring an additional transfer from your address to send extra tokens so the input is more than expected for the estimated output), it affects the input and output amount that you agree for signing the transaction. In many cases, the transaction cannot meet the input and output requirements because of the tax.

### Swapping with Transaction Fees

Before you swap any tokens, make sure you have visited their website to understand if they have a transaction fee mechanism (or _tax_ as many projects put it). If there is, make sure you set a slippage that is sufficient to accommodate the transaction fee -- e.g. if there is a transaction fee of 5%, your slippage will have to be set at at least 5% plus the normal trading slippage depending on your trading amount and the token's liquidity, say 5.5%-6%.&#x20;

In some extreme cases including some scams, some tokens even have a block on most or all transfers on chain, or only allowing certain addresses to sell, in such case it is impossible to swap the token successfully. Do learn about the token you are trying to swap and be aware of any fees and restrictions!
