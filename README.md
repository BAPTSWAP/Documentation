---
description: Docs in the making, not final version
---

# 👋 Introduction to Baptswap

<figure><img src=".gitbook/assets/intro.png" alt=""><figcaption></figcaption></figure>

### Overview

The Baptswap protocol is a peer-to-peer system, more commonly known as a Decentralized Exchange (DEX), designed for exchanging cryptocurrencies on the [Aptos Network](https://aptosfoundation.org/). Baptswap is designed to be secure, and function without any trusted intermediaries who may selectively restrict access.

Baptswap is the only protocol operating on MOVE-based blockchains allowing token owners to add fee-on-transfer solutions to their token swaps. Baptswap operates on the Aptos Network, meaning Aptos is the only MOVE-based blockchain to offer such “EVM-like” utility, while maintaining the flexiblity and scalability of the MOVE-language.&#x20;

There are currently two versions of the Baptswap protocol. V1 and V2 are open source, and are viewable [here](https://github.com/BAPTSWAP). Each version of Baptswap, once deployed, will function in perpetuity, with 100% uptime, provided the continued existence of the Aptos Network.

### How does the Baptswap protocol compare to a typical market?[​](https://docs.uniswap.org/concepts/uniswap-protocol#how-does-the-uniswap-protocol-compare-to-a-typical-market) <a href="#how-does-the-uniswap-protocol-compare-to-a-typical-market" id="how-does-the-uniswap-protocol-compare-to-a-typical-market"></a>

To understand how the Baptswap protocol differs from a traditional exchange, it is helpful to first look at two subjects: how the Automated Market Maker design deviates from traditional central limit order book-based exchanges, and how permissionless systems depart from conventional permissioned systems.

#### Order Book VS AMM[​](https://docs.uniswap.org/concepts/uniswap-protocol#order-book-vs-amm) <a href="#order-book-vs-amm" id="order-book-vs-amm"></a>

Most publicly accessible markets use a central limit [order book](https://www.investopedia.com/terms/o/order-book.asp) style of exchange, where buyers and sellers create orders organized by price level that are progressively filled as demand shifts. Anyone who has traded stocks through brokerage firms will be familiar with an order book system.

The Baptswap protocol takes a different approach, using an Automated Market Maker (AMM), sometimes referred to as a Constant Function Market Maker, in place of an order book.

At a very high level, an AMM replaces the buy and sell orders in an order book market with a liquidity pool of two assets, both valued relative to each other. As one asset is traded for the other, the relative prices of the two assets shift, and a new market rate for both is determined. In this dynamic, a buyer or seller trades directly with the pool, rather than with specific orders left by other parties. The advantages and disadvantages of Automated Market Makers versus their traditional order book counterparts are under active research by a growing number of parties.

#### Permissionless Systems[​](https://docs.uniswap.org/concepts/uniswap-protocol#permissionless-systems) <a href="#permissionless-systems" id="permissionless-systems"></a>

The second departure from traditional markets is the permissionless and immutable design of the Baptswap protocol. These design decisions were inspired by Uniswap Labs', on the Ethereum blockchain, commitment to the ideals of permissionless access and immutability as indispensable components of a future in which anyone in the world can access financial services without fear of discrimination or counter-party risk.

Permissionless design means that the protocol's services are entirely open for public use, with no ability to selectively restrict who can or cannot use them. Anyone can swap, provide liquidity, or create new markets at will. This is a departure from traditional financial services, which typically restrict access based on geography, wealth status, and age.

No party is able to pause the contracts, reverse trade execution, or otherwise change the behavior of the protocol in any way. It is worth noting that the coming Baptswap Governance will have the right (but no obligation) to change the amount of swap fees . However, this capability is known to all participants in advance, and to prevent abuse, the percentage is constrained between 0% and 0.9%.

### Where can I find more information[​](https://docs.uniswap.org/concepts/uniswap-protocol#where-can-i-find-more-information)? <a href="#where-can-i-find-more-information" id="where-can-i-find-more-information"></a>

For how Baptswap compare to other AMMs on Aptos, read more about its [unique features](introduction-to-baptswap/made-to-stand-out.md).

For research into the economics of AMMs, game theory, or optimization research, check out our research page once it is published.

For new features implemented in V2 that expand and refine the AMM design, see the [V2 Concepts](baptswap-v2/protocol-overview/) page.
