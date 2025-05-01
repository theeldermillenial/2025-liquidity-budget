# Cardano Treasury DeFi Liquidity Budget

## Abstract

The goal of this proposal is to increase liquidity on Cardano, specifically by supporting stablecoin liquidity. 50,000,000 ADA is requested over the course of 12 months to support the Cardano decentralized finance (DeFi) ecosystem. The majority of the funds in this budget will be disbursed to DeFi protocols including decentralized exchanges (DEXs) and lending protocols to help seed liquidity on Cardano. The funds are managed by a 7 person committee composed of publicly identified individuals who are part of multi-signature (multisig) wallet from which liquidity will be managed. This budget is proposed independent of other efforts since the goal of this budget is not to pay developers or companies for ecosystem improvements, rather to increase liquidity in the system overall. Further, unlike other proposals this budget serves as a revenue stream for the Cardano treasury since yields from DeFi protocols will be sent back to the Cardano treasury.

## Motivation

### Introduction

Liquidity is essential for any thriving blockchain ecosystem. Cardano has a developing ecosystem with many of the necessary primitives already built out: decentralized exchanges (DEXs), native stablecoins, money market protocols including borrow/lend and collateralized debt positions (CDP), and liquid staking tokens. Each of these primitives on their own help push an ecosystem from the development stage into the flourishing and mature stage. Stablecoins play a unique role in any cryptocurrency system as a means of onboarding new users with a fiat pegged token and volatility protection. However, without deep liquidity the true value of the Cardano decentralized finance (DeFi) ecosystem cannot be realized, and a critical mass of liquidity is necessary to encourage broader adoption. This proposal outlines the use of treasury funds to boost stablecoin liquidity, creating a stronger foundation for DeFi. Increasing stablecoin reserves not only expands liquidity but also attracts new users and reinforces confidence in the chain — offering a solid hedge against volatility and supports Cardano native stablecoins.

### High Level Overview

* **Amount** - The Cardano treasury should dedicate 3.33% of treasury funds (50 million ada) to purchasing fiat backed stablecoins, spread out over 12 monthly purchases.
* **Administration** - A 7 person committee will manage the treasury reserve using a multisig wallet (4 of 7 signature validation) to hold and deploy funds to protocols. The committee will be responsible for working with stablecoin issuers to convert ADA to fiat backed stablecoins and deploying liquidity. A specific focus of the committee will be analyzing approaches of deploying ADA to stablecoins in a way that minimizes ADA price impact.
* **Revenue** - ADA in the reserve waiting for deployment will be staked to earn interest while deployed over the 12 month period. 15% of fees generated from protocols will be withdrawn from the respective protocols and sent back to the treasury, while the remaining 85% of fees will remain in the protocol to accumulate.
* **Deployment** - DeFi protocols with at least 250,000 ADA worth of a stablecoin may apply to be recipients of minted stablecoin. A maximum of 2 or 3 protocols may be used per DeFi category to help minimize fragmentation. Applicants should make a strong case for the use of their protocol, including a a description of historical success, security, dedicated support for handling issues, and features of the protocol that will maximize the value to the Cardano treasury if liquidity is deployed to the protocol. New protocols will not be excluded for having limited history, but must make a strong case in other areas of the application.
* **Strategy** - The committee will deploy funds on a monthly basis in a way that minimizes ADA price impact and fees. A specific focus should be on deployment of liquidity that can be "passively" managed, meaning frequent adjustements are not needed.
* **Transparency** - The committee is responsible for either creating a monthly report or building a dashboard (or both) to describe the ADA held in reserve, the funds deployed to protocols, and all fees and other costs associated with managing the treasury. The committee may use part of the monthly budget to develop a dashboard to provide live updates of the stablecoin reserve for the Cardano community.
* **Costs** - Each member of the committee will be compensated $2,000/month (or can optionally be returned) in the fiat backed stablecoin of their choice ($14,000/month total for all committee members). The stablecoin reserve fund will cover the costs of minting fiat backed stables, deployment of liquidity to protocols, and rebalancing if needed. The committe will also use some funds to perform KYB/KYC of 3rd parties as needed as well as cover costs for creation of a legal entity to house the fund. Total costs per month should be capped at $50,000/month.
* **Organization** - Part of the initial budget will be used to investigate proper incorporation of a legal entity to house the funds being managed for this budget. Every reasonable attempt should be made to house the fund in a non-profit to maximize tax benefits as well as provide future opportunities for organizations to donate to the fund.
* **Revisions** - Since this fund may exist in perpetuity due to funds not being directly spent, it is important to have a mechanism for modification up to and including returning all funds back to the treasury. To this end, any member of the Cardano community may submit an Info Action to modify any aspect of this budget including members of the committee, monthly budget limits, committee pay, and returning some or all of funds back to the treasury. All members of the committee must commit to following any Info Action that is passed by 67% of the community vote. If a committee member does feel they can continue with their duties at any time, they must continue to carry out their duties until a suitable replacement is found according to the impeachment and replacement mechanisms.

### Governing Committee

#### Term Limits

Community members have a maximum term limit of 2 years, after which they can re-apply for a second 2 year term. A minimum of 4 community members (not affiliated with founding entities) must be on the committee at all times.

Founding entities may have at most 1 person each on the committee. There are no term limits for committee members that represent a founding entity, but must still abide by the removal process of an Info Action or a majority vote of the other committee members.

#### Retirement and Impeachment

In the event that a committee member retires or their signing keys are exposed, the remaining members of the committee must create a new multisig address with the same policy (4 of 7) that removes the retired address. This process also gives the committee the capacity to impeach inactive members of the committee, as well as the ability for the community to impeach one or more members through an info action.

## Rationale

### Constitutionality of the Budget

In compliance with **Article III Section** of the Cardano Constitution, this proposal contains a Title, Abstract, Reason for Proposal (Motivation and Rationale), and Supporting Materials. An off-chain copy of this proposal is linked to as the last element of the Supporting Materials section and is a Github link with commit hash thus fulfilling the other requirement of this section to have an off-chain copy with document hash. The Supporting Materials is not included in Github version of the document since it contains the commit hash.

In line with **Article IV Section 1** of the Cardano Constitution, we propose that this budget span 73 epochs (roughly 1 calendar year).

In compliance with **Article IV Section 2** of the Cardano Constitution, disbursements for this budget must be made to a multi-signature (multisig) wallet composed of at least seven independent members with at 4 of 7 signing policy. The process of overseeing funds then requires 4 of the 7 independent members committing to disbursement of funds to DeFi protocols. The wallet must be the owner of any liquidity deposited into DeFi protocols, meaning liquidity tokens or any other assurance of liquidity must be held in the multisig wallet and should not be delegated to a third party. With this design, the committee will be the administrator of the budget funds and will directly oversee distribution of funds to protocols. Each member of the committee must be publicly identified, and this in combination with the 4 of 7 signing policy protects against potential abuse.

At the time of submission, the NCL is currently at 350 million ADA and there are no other budgets that have been submitted on chain through an info action. We believe that this removes a potential constitutional barrier for this propsoal based on **Article IV Section 3**, since this proposal requests 50 million ADA and there are currently no competing budgets.

In compliance with **Article IV Section 4** of the constitution, we budget 2,000 ADA/month (24,000 ADA total) to cover the costs of audits and transparency. The building of a dashboard and quarterly reporting in the proposed work also fulfill the obligations of this section.

The nature of the proposed work fulfills the first requirement of **Article IV Section 5** of the constitution. The holding of all assets in the multisig account composed of 7 independent signers improves the ability of the Cardano community to easily audit and track actions taken by the committee. To fulfill the second part of the section, funds will not be delegated to an SPO and will be delegated to the predefined auto-abstain voting option.
