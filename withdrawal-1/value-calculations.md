# Value Calculations

## Summary

The purpose of this document is to describe the methods used to calculate value for the DeFi Liquidity Budget. The primary goal of the DeFi Liquidity Budget is to increase liquidity in the ecosystem, with a secondary goal of providing revenue back to the treasury. Thus, value tracking serves 2 purposes:

1. Reporting to show the status of the liquidity over time  
2. A means to calculate the revenue to send back to the treasury

This document will begin with a definition of terms and general concepts, an explanation of how the value of liquidity in different protocols are calculated, and finally examples of how a monthly revenue calculation will be performed (including amounts sent back to the treasury).

This document is NOT intended to be exhaustive, because every protocol operates slightly differently. It may be necessary to modify the calculations presented here based on the specific protocol mechanics. Thus, these calculations cover two general cases (lending and decentralized exchanges) based on how most protocols operate.

## Definitions and Concepts

Almost all protocols on Cardano use liquidity tokens to represent a liquidity position on Cardano. A liquidity provider deposits some form of liquidity (i.e. ADA, USDM, USDA, etc), and they receive liquidity tokens that represent the value of the deposit. Protocols generally identify the change in value of these tokens based on the change in underlying pooled liquidity.

For an example of how this works on a DEX, if a liquidity provider deposits 1000 ADA and 1000 USDM into a liquidity pool, they will receive 1,000,000 liquidity tokens (numbers are used for illustration of the concept). After several days of trading, the liquidity provider still has 1,000,000 liquidity tokens, but when redeeming the liquidity tokens they might receive 1001 ADA and 1001 USDM assuming there was no impermanent loss. This means that the 1,000,000 liquidity tokens grew in value by \~0.1%.

For an example of how this works on a lending protocol, a liquidity provider might deposit 1000 ADA into a liquidity pool and receive 1000 liquidity tokens. As the tokens are loaned out, and the loans are repaid, the pool of ADA will grow but the number of liquidity tokens might remain static. When the liquidity provider redeems their liquidity tokens, they might trade in their 1000 liquidity tokens for 1001 ADA, representing 0.1% increase in the liquidity tokens value.

Thus, to calculate the increase in liquidity value, it is often sufficient to calculate the value of the liquidity tokens. However, there is a large difference in how lending liquidity value and DEX liquidity value are calculated. This is because DEX liquidity value is susceptible to impermanent loss. Impermanent loss occurs when the price ratio of tokens in a liquidity pool changes relative to when they were deposited, causing the value of the position to be less than if the tokens were simply held. For example, if a liquidity provider deposits equal values of ADA and USDM and ADA's price doubles, the pool rebalances to hold more USDM and less ADA, resulting in less total value than holding the original tokens outside the pool. When there is impermanent loss, calculating value usually requires calculating the value in one token denomination and subtracting or adding the impact of the overall price change. Lending protocols have a similar impermanent loss for non-fiat backed tokens. For example, if ADA is deposited then the total value of the liquidity tokens is a combination of the increase in total ADA value of the liquidity tokens plus the change in the price of ADA over time.

In this document, we will consider two narrowly focused scenarios that directly apply to the use cases of the Cardano DeFi Liquidity Budget. The first is the lending value of fiat backed stablecoins, and the second is the value of ADA/Stablecoin pairs or Stablecoin/Stablecoin pairs deposited into DEX protocols. For DEX liquidity value, we use an impermanent loss agnostic metric for calculating value.

## Calculation of Liquidity Value

### Lending Protocols

For lending protocols, we assume only fiat backed stablecoins are deposited into liquidity pools. Assuming fiat backed stablecoins are equivalent to a dollar, since they can be redeemed 1 token for $1, the calculation of value increase will be assessed directly by the increase of liquidity token value in tokens:

Value Change Percentage \= L\_b / L\_a \- 1 \= V\_l

Here, L\_a is the liquidity token value at the beginning of the month and L\_b is the token value at the end of the month denominated in stablecoin value. V\_l will represent the change in value of liquidity tokens for a lending protocol, and will use this value below when discussing capitalization and treasury revenue.

### DEX Protocols

For DEX protocols that use ADA/Stablecoin measurements, we use an impermanent loss agnostic (ILA) measurement of value increase. We will briefly discuss below the potential pitfalls and reasons to still use this metric in spite of them. The formula for the ILA measurement is:

Value Change Percentage \= √(X\_b \* Y\_b) / √(X\_a \* Y\_a) \- 1 \= V\_cpp

X\_a and  Y\_a represent the total number of tokens in the pool at the beginning of the month, X\_b and Y\_b represent the total number of tokens in a liquidity pool at the end of the month, and V\_cpp represents the change in value for constant product pools (CPP) on DEXs.

The fundamental equation used for CPP is to simply multiply the total number of tokens in the pool. When depositing or withdrawing liquidity, the product of tokens X and Y are required to be the same. When swapping, the product is also required to be the same with a small increase in the total product commensurate with the fees charged by the pool. The V\_cpp value is calculated by taking the square root of the product at the end of the month and dividing by the square root of the product at the beginning of the month. Since the product of the pair can only increase due to swapping (and remain unchanged when depositing or withdrawing), the value of this ratio can only increase. Taking the square root of each value casts the function onto a linear scale, permitting the ratio of the square root of products to a unitless measure of liquidity value increase.

NOTE: It is important to understand that V\_cpp does not account for permanent loss. However, the nature of the calculation is such that if the value calculated by V\_cpp were to be removed after an extreme price movement, a price recovery would result in a restoration of the full original liquidity value (plus interest gained for the swaps required for the price recovery). This means that removal of less than V\_cpp in total value will not result in dipping into the value of the original deposit if the price were to recover.

NOTE: V\_cpp does not cover the case of stableswaps. In the case of stableswaps where all tokens in the pair are fiat backed stablecoins, a modification of the representative token sum can be used to calculate the change in value.

### Capitalization and Revenue

At the end of each month, the value of all liquidity tokens will be captured and used to calculate the total increase in value relative to the value of liquidity tokens at the beginning of the month. The absolute value increase will be calculated in liquidity token units:

VT\_l \= V\_l \* T\_l

VT\_cpp \= V\_cpp \* T\_cpp

VT\_l and VT\_cpp represent the increase in value denominated in liquidity tokens, and T\_l and T\_cpp represent the total number of liquidity tokens owned at the end of the month.

As defined in the governance protocol for the DeFi Liquidity Budget, 15% of the value increase will be sent back to the treasury. Thus, the total treasury revenue will be:

R \= (0.15 \* VT\_l1 \+ 0.15 \* VT\_l2 \+ 0.15 \* VT\_cpp1 \+ 0.15 \* VT\_cpp2)

VT\_l1 and VT\_l2 are the total token value increase for two different lending protocols, and VT\_cpp1 and VT\_cpp2 are the total token value increases for two different DEXs. R is the composite number of each liquidity token that should be removed, liquidated, and sent back to the treasury.Thus, revenue represents multiple liquidity assets that will need to be converted to ADA and sent back to the treasury.

The remaining 85% will be used to pay committee members and any other costs, and the remainder is left in the protocol to compound. There is an explicit rule in the governance protocol that 6 months post launch of liquidity, costs in excess of 85% result in committee members receiving lesser pay. This is to protect the starting capital deposited into the ecosystem, because as described above, taking out more than the value change percentage would result in a decrease in the original investment.  
