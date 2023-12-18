# Fee Structure on Baptswap

## Introduction

Understanding the fee structure is crucial for participants in the Baptswap ecosystem. This page outlines the different types of fees involved in token swaps and liquidity provision, and how they are allocated.

## Liquidity Provider Fees

### Swapping Fee

A 0.9% fee is applied to token swaps. From this, 0.3% is distributed among liquidity providers in proportion to their contribution to the liquidity reserves. The remaining portion of this fee is also allocated to the Baptswap Treasury as a Protocol Fee.

### Fee Tiers

All tokens launching on Baptswap, will have a default swapping fee of 0.9%. However, the protocol may add several fee tiers, lowering the fees for frequently traded pairs.

### Fee Allocation

Swapping fees are directly added to the liquidity reserves, thereby increasing the value of liquidity tokens.

Liquidity providers collect their portion of the fees by burning liquidity tokens, which withdraws their share of the underlying reserves.

### Impact on Liquidity Pools

With each trade, the fees added to the pool increase the invariant (`token0_pool / token1_pool`) from the end of the previous transaction.

### Calculating LP Returns

**Tools and Resources**: Various community-developed tools are available to help determine LP returns. Further information on understanding LP returns can be found in the Baptswap documentation.

## Protocol Fees

### Current Protocol Fee

Currently, the Protocol Fee is set at 0.60% for pools with 0.90% Swapping Fees. The Protocol Fees goes to the Treasury, and is allocated for the growth of Baptswap.

This fee may be subject to change, with the possibility of being reduced or turned off in the future.

## More Information

Details on potential future changes to the Protocol Fee will be available in upcoming blog posts.
