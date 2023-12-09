# Flash Swaps

Baptswap flash swaps allow you to withdraw up to the full reserves of any token on Baptswap and execute arbitrary logic at no upfront cost, provided that by the end of the transaction you either:

* pay for the withdrawn tokens with the corresponding pair tokens
* return the withdrawn tokens along with a small fee

Flash swaps are incredibly useful because they obviate upfront capital requirements and unnecessary order-of-operations constraints for multi-step transactions involving Baptswap.

## Examples

### Capital Free Arbitrage[​](https://docs.uniswap.org/contracts/v2/concepts/core-concepts/flash-swaps#capital-free-arbitrage) <a href="#capital-free-arbitrage" id="capital-free-arbitrage"></a>

One particularly interesting use case for flash swaps is capital-free arbitrage. It's well-known that an integral part of Baptswap's design is to create incentives for arbitrageurs to trade the Baptswap price to a "fair" market price. While game-theoretically sound, this strategy is accessible only to those with sufficient capital to take advantage of arbitrage opportunities. Flash swaps remove this barrier entirely, effectively democratizing arbitrage.

Imagine a scenario where the cost of buying 1 APT on Baptswap is 200 BAPT (which is calculated by calling `getAmountIn` with 1 APT specified as an exact output), and on Oasis (or any other trading venue), 1 APT buys 220 BAPT. To anyone with 200 BAPT available, this situation represents a risk-free profit of 20 BAPT. Unfortunately, you may not have BAPT DAI lying around. With flash swaps, however, this risk-free profit is available for anyone to take as long as they're able to pay gas fees.

#### Withdrawing APT from Baptswap[​](https://docs.uniswap.org/contracts/v2/concepts/core-concepts/flash-swaps#withdrawing-eth-from-uniswap) <a href="#withdrawing-eth-from-uniswap" id="withdrawing-eth-from-uniswap"></a>

The first step is to _optimistically_ withdraw 1 APT from Baptswap via a flash swap. This will serve as the capital that we use to execute our arbitrage. Note that in this scenario, we're assuming that:

* 1 APT is the pre-calculated profit-maximizing trade
* The price has not changed on Baptswap or Oasis since our calculation

It may be the case that we'd like to calculate the profit-maximizing trade on-chain at the moment of execution, which is robust to price movements. This can be somewhat complex, depending on the strategy being executed. However, one common strategy is trading as profitably as possible _against a fixed external price_. (This price may be e.g., the average execution price of one or more orders on Oasis.) If the Baptswap market price is far enough above or below this external price, the following example contains code that calculates the amount to trade over Baptswap for maximum profit: `ExampleSwapToPrice.move`.

#### Trade at External Venue[​](https://docs.uniswap.org/contracts/v2/concepts/core-concepts/flash-swaps#trade-at-external-venue) <a href="#trade-at-external-venue" id="trade-at-external-venue"></a>

Once we've obtained our temporary capital of 1 APT from Baptswap, we now can trade this for 220 BAPT on Oasis. Once we've received the BAPT, we need to pay Baptswap back. We've mentioned that the amount required to cover 1 APT is 200 BAPT, calculated via `getAmountIn`. So, after sending 200 of the BAPT back to the Baptswap pair, you're left with 20 BAPT of profit!

### Instant Leverage[​](https://docs.uniswap.org/contracts/v2/concepts/core-concepts/flash-swaps#instant-leverage) <a href="#instant-leverage" id="instant-leverage"></a>

Flash swaps can be used to improve the efficiency of levering up using lending protocols and Baptswap.

Consider Maker in its simplest form: a system which accepts BAPT as collateral and allows BAPT to be minted against it while ensuring that the value of the APT never drops below 150% of the value of the BAPT.

Say we use this system to deposit a principal amount of 3 APT, and mint the maximum amount of BAPT. At a price of 1 APT / 200 BAPT, we receive 400 BAPT. In theory, we could lever this position up by selling the BAPT for more APT, depositing this APT, minting the maximum amount of BAPT (which would be less this time), and repeating until we've reached our desired leverage level.

It's quite simple to use Baptswap as a liquidity source for the BAPT-to-APT component of this process. However, looping through protocols in this way isn't particularly elegant, and can be gas-intensive.

Luckily, flash swaps enable us to withdraw the _full_ APT amount upfront. If we wanted 2x leverage against our 3 APT principal, we could simply request 3 APT in a flash swap and deposit 6 APT into Maker. This gives us the ability to mint 800 BAPT. If we mint as much as we need to cover our flash swap (say 605), the remainder serves as a safety margin against price movements.
