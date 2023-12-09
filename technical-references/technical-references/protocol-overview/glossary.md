# Glossary

#### Automated market maker[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#automated-market-maker) <a href="#automated-market-maker" id="automated-market-maker"></a>

An automated market maker is a smart contract on Ethereum that holds on-chain liquidity reserves. Users can trade against these reserves at prices set by an automated market making formula.

#### Constant product formula[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#constant-product-formula) <a href="#constant-product-formula" id="constant-product-formula"></a>

The automated market making algorithm used by Baptswap.

#### Factory[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#factory) <a href="#factory" id="factory"></a>

A smart contract that deploys a unique smart contract for any trading pair on Aptos.

#### Pair[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#pair) <a href="#pair" id="pair"></a>

A smart contract deployed from the Baptswap V2 Factory that enables trading between two tokens.

#### Pool[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#pool) <a href="#pool" id="pool"></a>

Liquidity within a pair is pooled across all liquidity providers.

#### Liquidity provider / LP[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#liquidity-provider--lp) <a href="#liquidity-provider--lp" id="liquidity-provider--lp"></a>

A liquidity provider is someone who deposits an equivalent value of two tokens into the liquidity pool within a pair. Liquidity providers take on price risk and are compensated with fees.

#### Mid price[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#mid-price) <a href="#mid-price" id="mid-price"></a>

The price between what users can buy and sell tokens at a given moment. In Baptswap this is the ratio of the two token reserves.

#### Price impact[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#price-impact) <a href="#price-impact" id="price-impact"></a>

The difference between the mid-price and the execution price of a trade.

#### Slippage[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#slippage) <a href="#slippage" id="slippage"></a>

The amount the price moves in a trading pair between when a transaction is submitted and when it is executed.

#### Core[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#core) <a href="#core" id="core"></a>

Smart contracts that are essential for Baptswap to exist. Upgrading to a new version of core would require a liquidity migration.

#### Periphery[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#periphery) <a href="#periphery" id="periphery"></a>

External smart contracts that are useful, but not required for Baptswap to exist. New periphery contracts can always be deployed without migrating liquidity.

#### Flash swap[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#flash-swap) <a href="#flash-swap" id="flash-swap"></a>

A trade that uses the tokens being purchased before paying for them.

#### `x * y = k`[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#x--y--k) <a href="#x--y--k" id="x--y--k"></a>

The constant product formula.

#### Invariant[​](https://docs.uniswap.org/contracts/v2/concepts/protocol-overview/glossary#invariant) <a href="#invariant" id="invariant"></a>

The "k" value in the constant product formula
