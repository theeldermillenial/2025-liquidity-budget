# Stablecoin DeFi Liquidity Budget

## Treasury Withdrawal Action 1

## Executive Summary

For the last year, we have engaged the Cardano community to discuss deployment of treasury funds into the DeFi ecosystem to boost liquidity. Under the old constitution, we received broad support (more than 67%) for a budget info action to deploy 50,000,000 ADA into the ecosystem. While we acknowledge a budget info action is not required under the current constitution, we feel encouraged to submit this withdrawal action to setup the legal and on chain components needed to carry out the liquidity deployment. For a detailed overview of what we are aiming to accomplish more broadly, we invite people to read the budget info action (gov_action1u4jrcvlkppjzuv5j9z5ksacwtvv77h6glu0knpcjut8gvjjfu0cqqt3alsy).

In this Withdrawal Action, we propose withdrawing 800,000 ADA to setup a legal entity and audit the smart contract that will be built free of charge courtesy of Lucas and Kasey from UTxO Company. The user interface will be contributed by Hinson from Sidan Labs.

## Terms of Withdrawal

### Purpose of Withdrawal

This withdrawal is intended solely for establishing the legal and technical infrastructure required to implement the Stablecoin DeFi Liquidity Budget approved by the Cardano Community. Specifically, funds will be used to:

1. Establish a Cayman Islands Foundation Company as the legal vehicle for fund management
2. Audit the administrating smart contract system (development is contributed at no cost by UTxO Company and Sidan Labs)
3. Deploy Amaru contract infrastructure for secure multisig fund management during this withdrawal period

### Period for Delivery

All activities funded by this withdrawal shall be completed within 6 months from the date funds are received by the Amaru contract. If any activity cannot be completed within that period, any outstanding funds allocated to that activity will be returned to the Cardano Treasury.

### Costs and Expenses

Maximum allocated costs for this withdrawal:

| Category | Maximum Allocation | Provider |
|----------|--------------------|----------|
| Legal Structure | 664,000 ADA max | Walkers (Cayman) LLP / Walkers Corporate Limited |
| Smart Contract Audit | 111,000 ADA | Invariant0 LLC |
| Amaru Contract Setup | 25,000 ADA | Sundae Labs |
| Smart Contract Development | 0 ADA | UTxO Company & Sidan Labs (contributed) |
| **Total** | **800,000 ADA** | |

Legal structure costs are denominated in USD. The Committee will withdraw only the ADA required to cover the USD value of invoices at the time of payment. Any ADA remaining after all legal obligations are settled will be returned to the Cardano Treasury. Audit and Amaru setup costs are fixed in ADA as stated.

### Circumstances for Refund to Treasury

Funds shall be refunded to the Cardano Treasury under the following circumstances:

1. **Service provider non-performance** — if any service provider fails to deliver agreed milestones, contracts are terminated for cause, or deliverables are rejected; any unspent funds allocated to that provider will be returned
2. **Cost savings** — if total actual costs are less than the allocated maximum; the Committee will notify the community of the amount and whether it is returned to the treasury or transferred to Withdrawal 2
3. **Legal formation impossibility** — if the Cayman Islands Foundation Company cannot be incorporated, if regulatory changes prevent the structure from functioning as intended, or if directors cannot be appointed
4. **Technical impossibility** — if the smart contract cannot be completed, if the security audit identifies critical unfixable vulnerabilities, or if the contract cannot meet constitutional requirements
5. **Governance changes** — if DReps vote to discontinue the project or if the Constitutional Committee determines the implementation is unconstitutional
6. **Completion with remainder** — upon successful completion of all deliverables, any remaining funds will be returned to the treasury or applied to Withdrawal 2 with explicit community notification

**Refund process:** The Committee will execute all refunds via the Amaru contract with 5-of-9 multisig approval, sending funds to the Cardano Treasury staking address. All refunds will be documented in the monthly transparency report with a full explanation of circumstances.

---

## 1\. Legal Structure

### 1.1 Why a Legal Entity Is Required

A legal entity is a prerequisite for managing treasury funds responsibly on behalf of the Cardano community, for three reasons. First, a legal entity has its own legal personality, meaning it can hold assets, enter contracts, and pursue or defend legal claims in court. Without this, the fund has no mechanism to recover misappropriated assets or enforce agreements with service providers, OTC desks, or DeFi protocols — all of whom require a recognized legal counterparty to transact. This is not a theoretical concern: the fund will need to work with regulated financial institutions that have strict KYC and AML obligations and cannot engage with an informal unincorporated group.

Second, without a legal entity, a group of individuals acting together to manage pooled funds may be characterized as a general partnership under the laws of many jurisdictions, exposing every member to joint and several personal liability for the group's obligations. This risk is not hypothetical. In *Sarcuni v. bZx DAO* (U.S. District Court, 2023) and *Samuels v. Lido DAO* (2024), courts found that unwrapped DAO participants could be held personally liable as general partners for the DAO's debts and obligations. A properly structured legal entity provides committee members with limited liability protection, allowing them to serve the community without risking personal financial ruin.

Third, a legal entity creates enforceable fiduciary obligations and formal accountability mechanisms that supplement on-chain governance. Directors and committee members operating under a legal structure have defined duties that the community — through the tDAO — can enforce. The Cayman Islands Foundation Company has emerged as the established industry standard for this purpose, used by leading DAOs including Aave and others, precisely because its memberless, director-led structure mirrors decentralized governance while providing the legal protections described above.

### 1.2 Service Provider

We will use Walkers LLP for establishment of the legal entity. While Walkers is a bit more costly, they have dedicated staff to handle regulatory issues which is unique among Cayman legal firms. Since we want this legal entity to survive in the long term and overcome any obstacles we see in the future, we decided to spend a little more to have additional protections in case questions of the non-profit status by regulators are questioned.

**Walkers (Cayman) LLP**  
**Location:** Cayman Islands  
**Website:** [walkersglobal.com](https://walkersglobal.com)

### 1.3 Legal Structure: Cayman Islands Foundation Company

The legal entity will be a **Cayman Islands Foundation Company (FC)** with the following characteristics:

**Key Features:**

- **Memberless, director-led structure** designed for DAO governance  
- **Separate legal personality** enabling the FC to hold assets, enter contracts, and act as legal counterparty for off-chain transactions  
- **Limited liability protection** for Committee Members and other participants  
- **Customizable governance** that mirrors on-chain tDAO and Committee structure  
- **No shareholders or beneficial owners**, aligning with decentralized governance principles

**Governance Structure:**

- **Directors:** Minimum 2 Cayman-based professional directors who manage the FC's business and affairs in accordance with the FC's Articles and tDAO directives  
- **Supervisor:** Cayman-based professional supervisor with enforcement rights to act as a check on directors  
- **Committee:** 9-person Interim Committee with delegated operational authority (5-of-9 multisig approval for fund disbursements)  
- **tDAO Oversight:** dReps retain power to appoint/remove Committee Members and shut down the fund via on-chain governance

**Director Candidates:**

- **Candidate \#1**: Co-founder of world's first Bitcoin ATM network; Founding President of Netcoins; Founding CEO of SonicStrategy; 15+ years in regulated crypto ventures  
- **Candidate \#2:** Leading one of the world’s largest crypto DeFi market makers; CFA & CFP; former senior global capital markets professional; Board Member & Treasurer, CFA Society Cayman Islands.

### 1.4 Implementation Plan

**Phase 1: Legal Formation**

1. Finalize FC name and conduct name check with Registrar of Companies  
2. Interview and appoint directors and supervisor  
3. Draft and review formation documents:  
   - Affidavit  
   - Memorandum and Articles of Association  
   - Undertaking of subscriber  
   - Subscriber resolutions  
   - Director service agreements  
   - Supervisor service agreement  
4. Incorporate the Foundation Company with Cayman Islands Registrar

**Phase 2: Activation**

1. Pass director resolutions to:  
   - Appoint the 9 Interim Committee Members  
   - Designate the smart contract wallet as an FC asset  
   - Approve 5-of-9 multisig governance structure  
   - Approve Committee Member service agreements (remuneration, indemnity, multisig arrangements)  
   - Approve transaction documents for liquidity deployment  
2. Establish banking relationships (if required)  
3. Complete regulatory filings

### 1.5 Detailed Cost Breakdown

| Service | Provider | Cost (USD) | Cost (ADA) @ $0.25/ADA |
| :---- | :---- | :---- | :---- |
| Constitutional documents & resolutions | Walkers (Cayman) LLP | $25,000 \- $30,000 | 100,000 \- 120,000 |
| Disbursements (filing fees, etc.) | Walkers (Cayman) LLP | $6,000 | 24,000 |
| Cayman regulatory memorandum | Walkers (Cayman) LLP | $12,500 | 50,000 |
| Transaction document review (est. 5 docs) | Walkers (Cayman) LLP | $7,500 \- $10,000 | 20,000 \- 40,000 |
| Registered office & secretary (Year 1\) | Walkers Corporate Limited | $10,000 | 40,000 |
| Supervisor services (Year 1\) | Walkers Corporate Limited | $20,000 | 80,000 |
| Director fees (Year 1, 2 directors est.) | See below | $50,000 | 200,000 |
| Contingency for additional legal work |  | $10,000 | 40,000 |
| **TOTAL LEGAL STRUCTURE** |  | **\~$166,000** | **\~664,000 ADA** |

**Notes:**

- ADA conversion calculated at $0.40/ADA. Actual ADA amount may vary based on exchange rate at time of payment.  
- Director fees are estimated; final amount depends on negotiated terms with selected directors.  
- Registered office and supervisor services are annual fees; only Year 1 costs included in this withdrawal.  
- Walkers Corporate Limited is an affiliate of Walkers LLP but provides services at competitive market rates. Alternative service providers may be considered if cost optimization is required.

---

## 3\. Smart Contract Audit

### 3.1 Service Provider

**Invariant0 LLC**  
**Website:** [https://invariant0.com](https://invariant0.com)  
**GitHub:**

- [https://github.com/vacuumlabs/audits](https://github.com/vacuumlabs/audits) (legacy reports)  
- [https://github.com/Invariant-0/audit-reports](https://github.com/Invariant-0/audit-reports) (current reports)

**Lead Auditor:** Michal Porubsky, Founder and Lead Auditor

### 3.2 Cost Breakdown

| Service | Provider | Cost | Notes |
| :---- | :---- | :---- | :---- |
| Design & Specification Review | Invariant0 LLC | Included | 3-4 days |
| Smart Contract Code Audit | Invariant0 LLC | Included | 12-16 days, 2 auditors |
| Re-audit of all fixes | Invariant0 LLC | Included | Iterative process |
| Final Audit Reports | Invariant0 LLC | Included | Internal \+ Public |
| **TOTAL AUDIT** |  | **111,000 ADA** | **Fixed Price** |

---

## 4\. Amaru Contract Setup

### 4.1 Service Provider

**Sundae Labs**  
**Website:** [https://sundae.fi](https://sundae.fi)  
**Supporting Role:**

- Additional technical support and consultation  
- Cardano smart contract expertise  
- Community integration support

### 4.2 Purpose

An Amaru contract will be established to receive the 800,000 ADA from this withdrawal and manage disbursements to service providers. This provides:

- Secure multi-signature control by the 9-person Interim Committee  
- Transparent on-chain tracking of all payments  
- Protection against single point of failure  
- Constitutional compliance with fund management requirements

### 4.3 Cost & Timeline

| Service | Provider | Cost | Timeline |
| :---- | :---- | :---- | :---- |
| Amaru contract setup & support | Sundae Labs | 25,000 ADA | 1-2 weeks |

---

## Prior Treasury Receipt Disclosure

In accordance with Article I, Section 7(2) of the Cardano Constitution, the prospective recipient of this withdrawal is the Stablecoin DeFi Liquidity Interim Committee, acting through an Amaru multisig contract requiring 5-of-9 signatures. The Stablecoin DeFi Liquidity Interim Committee has not received ada from the Cardano Treasury within the last 24 months.

---

## 5\. Constitutional Compliance Summary

This withdrawal action complies with all applicable sections of the Cardano Constitution (ratified 2025).

### Article I, Section 6 \- Governance Action Standards

This action follows the standardized format required by Article I, Section 6:

- **Title, abstract, justification, and supporting materials** — provided in this document
- **URL and document hash** — to be added prior to on-chain submission
- **On-chain content identical to final off-chain version** — this document is the off-chain specification; the on-chain metadata will match exactly

All smart contract code will be published to a public GitHub repository, enabling full community verification of deliverables.

### Article I, Section 7 \- "Treasury Withdrawals" Action Standards

**Section 7(1) — Terms of withdrawal**

The Terms of Withdrawal section above specifies: the purpose of the withdrawal, the period for delivery of all proposed activities (6 months), the relevant costs and expenses for each component, and the circumstances under which funds will be refunded to the Cardano Treasury.

**Section 7(2) — Prior treasury receipt disclosure**

Addressed in the Prior Treasury Receipt Disclosure section above. The Stablecoin DeFi Liquidity Interim Committee has not received ada from the Cardano Treasury within the last 24 months.

**Section 7(3) — Net Change Limit**

This withdrawal does not exceed the Net Change Limit. As of submission, the NCL is approximately 350 million ADA; this withdrawal represents approximately 0.23% of the NCL. (800,000 ADA / 350,000,000 ADA NCL)

**Section 7(4) — Audit allocation and oversight metrics**

- 75,000 ADA is allocated for an independent security audit of the smart contract by Invariant0 LLC, covering design review, code audit, fix re-auditing, and public and internal final reports
- Periodic independent audits of fund usage are addressed in the approved Governance Protocol and will be funded from Withdrawal 2 operational budget or fund revenue
- The following oversight metrics will be implemented and published monthly on the Cardano governance forum:
  - Total funds held in the Amaru contract and disbursed to each service provider
  - Milestone completion status for each service provider
  - Cost variance between budgeted and actual expenditures
  - Timeline adherence and any delays with explanations
  - All on-chain transactions publicly verifiable via the Amaru contract address

**Section 7(5) — Designated administrators**

The nine-person Interim Committee serves as the designated administrators for this withdrawal, responsible for monitoring fund use and ensuring deliverables are achieved:

- Review and approve all service provider invoices against agreed milestones before releasing payment
- Verify that deliverables meet specifications (legal entity properly incorporated; smart contract code open-sourced and audited; audit reports published)
- Track progress against the delivery timeline in the Terms of Withdrawal
- Report monthly to the Cardano Community on all expenditures and progress
- Execute any required refunds to the treasury via 5-of-9 multisig

The 5-of-9 multisig requirement distributes oversight across all nine committee members; no single member can authorize a disbursement. The tDAO retains on-chain oversight through its ability to impeach committee members and disable contract actions at any time.

Committee members (as identified in the approved Info Action):
Linda Roland, Darren Camas, Nick Schaub Ph.D., Giorgio Zinetti, Massimo Morini Ph.D., Darlington Wleh, Murasaki, Raphael Christian-Roy, Ryan Davis.

**Section 7(6) — Fund management**

- All withdrawn ada is held in the Amaru multisig contract, a separate auditable account publicly verifiable on the Cardano blockchain
- Funds are not delegated to any SPO
- Funds are delegated to the predefined abstain voting option per Article I, Section 7(6)

### Treasury Guardrails (Appendix I, Section 3\)

**TREASURY-01a** — A Net Change Limit has been agreed by DReps via on-chain governance action  
**TREASURY-02a** — This withdrawal does not exceed the Net Change Limit  
**TREASURY-03a** — This withdrawal is denominated in ada  
