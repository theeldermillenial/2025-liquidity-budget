# Stablecoin DeFi Liquidity Budget

## Treasury Withdrawal Action 1

## Executive Summary

As outline in the DeFi Liquidity Budget Info Action, this first withdrawal action requests 500,000 ADA from the Cardano Treasury to establish the legal framework and smart contract infrastructure required for the Stablecoin DeFi Liquidity Budget as approved by the Cardano Community. This withdrawal covers three critical components: (1) establishment of a Cayman Islands Foundation Company as the legal vehicle for fund management, (2) development of the administrating smart contract and user interfaces, and (3) comprehensive security audit of the smart contract system.

All funds will be initially received by an Amaru contract administered by the 9-person Interim Committee with a 5-of-9 multisignature requirement. Funds will be disbursed to service providers upon completion of agreed milestones as detailed in this proposal.

---

## 1\. Legal Structure

### 1.1 Service Provider

**Walkers (Cayman) LLP**  
**Location:** Cayman Islands  
**Website:** [walkersglobal.com](https://walkersglobal.com)

### 1.2 Legal Structure: Cayman Islands Foundation Company

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

### 1.3 Implementation Plan

**Phase 1: Legal Formation (3-5 weeks)**

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

**Phase 2: Activation (1-2 weeks)**

1. Pass director resolutions to:  
   - Appoint the 9 Interim Committee Members  
   - Designate the smart contract wallet as an FC asset  
   - Approve 5-of-9 multisig governance structure  
   - Approve Committee Member service agreements (remuneration, indemnity, multisig arrangements)  
   - Approve transaction documents for liquidity deployment  
2. Establish banking relationships (if required)  
3. Complete regulatory filings

### 1.4 Detailed Cost Breakdown

| Service | Provider | Cost (USD) | Cost (ADA) @ $0.40/ADA |
| :---- | :---- | :---- | :---- |
| Constitutional documents & resolutions | Walkers (Cayman) LLP | $25,000 \- $30,000 | 62,500 \- 75,000 |
| Disbursements (filing fees, etc.) | Walkers (Cayman) LLP | $6,000 | 15,000 |
| Cayman regulatory memorandum | Walkers (Cayman) LLP | $12,500 | 31,250 |
| Transaction document review (est. 5 docs) | Walkers (Cayman) LLP | $7,500 \- $10,000 | 18,750 \- 25,000 |
| Registered office & secretary (Year 1\) | Walkers Corporate Limited | $10,000 | 25,000 |
| Supervisor services (Year 1\) | Walkers Corporate Limited | $20,000 | 50,000 |
| Director fees (Year 1, 2 directors est.) | See below | $50,000 | 125,000 |
| Contingency for additional legal work |  | $10,000 | 25,000 |
| **TOTAL LEGAL STRUCTURE** |  | **\~$166,000** | **\~400,000 ADA** |

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
| **TOTAL AUDIT** |  | **75,000 ADA** | **Fixed Price** |

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

An Amaru contract will be established to receive the 500,000 ADA from this withdrawal and manage disbursements to service providers. This provides:

- Secure multi-signature control by the 9-person Interim Committee  
- Transparent on-chain tracking of all payments  
- Protection against single point of failure  
- Constitutional compliance with fund management requirements

### 4.3 Cost & Timeline

| Service | Provider | Cost | Timeline |
| :---- | :---- | :---- | :---- |
| Amaru contract setup & support | Sundae Labs | 25,000 ADA | 1-2 weeks |

---

## 5\. Constitutional Compliance Summary

This withdrawal action complies with all relevant sections of the Cardano Constitution:

### Article III, Section 5 \- Transparency Requirements

**Title, Abstract, Reason, Supporting Materials** \- Provided in this document  
**URL and hash** \- Will be added with final submission  
**Off-chain content** \- This document serves as complete off-chain specification

**Open source development** \- All smart contract code will be publicly available on GitHub for public review  
**Documentation** \- Comprehensive documentation will enable community verification of all components

### Article IV, Section 2 \- Budget Administration

**Smart contract based administration:**

- Amaru contract for Withdrawal 1 fund management  
- Custom administrating contract for Withdrawal 2 liquidity deployment  
- Smart contract enforces 5-of-9 spending requirement

**Designated administrators:**

- 9-person Interim Committee with 5-of-9 multisig approval required for all disbursements  
- FC governance structure mirrors on-chain tDAO oversight mechanisms

**Oversight process:**

- Monthly reporting of all expenditures and progress  
- tDAO oversight via on-chain governance actions  
- tDAO implemented on-chain with election, impeachment, and shutdown capabilities

**Asset custody:**

- Smart contract will hold all liquidity tokens  
- All liquidity tokens held by smart contract (not delegated to third parties)

### Article IV, Section 3 \- Treasury Withdrawal Limits

**Within net change limit** \- 500,000 ADA is well below current NCL (\~350M ADA)  
**Authorized by approved budget** \- Pursuant to passed Info Action (Stablecoin DeFi Liquidity Budget)  
**Not unconstitutional** \- Complies with all constitutional requirements as detailed in this document

### Article IV, Section 4 \- Audit & Dispute Resolution

**Audit allocation:**

- 75,000 ADA allocated for comprehensive security audit by Invariant0 LLC  
- Independent third-party audit by experienced Cardano smart contract auditors  
- Comprehensive security review of all contract logic  
- Public audit report for community transparency  
- Audit costs included in withdrawal budget

**Dispute resolution provisions:**

- All service agreements include arbitration provisions  
- Director service agreements will include dispute resolution procedures  
- Committee Member agreements will include dispute resolution provisions  
- FC Articles will include dispute resolution mechanisms for entity-level disputes

### Article IV, Section 5 \- Fund Management

**Separate auditable accounts:**

- All funds held in separate, auditable smart contract addresses  
- Amaru contract provides public on-chain transparency for Withdrawal 1  
- All transactions publicly verifiable on Cardano blockchain

**Delegation requirements:**

- Funds will NOT be delegated to any SPO  
- Explicitly prohibited in contract configuration  
- Funds will be delegated to predefined auto-abstain voting option per constitutional requirement

### Treasury Guardrails (Appendix I, Section 3\)

**TREASURY-03a \- Denomination** \- All withdrawals denominated in ADA  
**TREASURY-04a \- Budget approval** \- Approved budget in effect via passed Info Action  
