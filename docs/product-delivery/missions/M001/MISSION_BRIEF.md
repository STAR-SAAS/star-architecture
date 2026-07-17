# [M001] Mission-001 · SmartQuote Foundation

> Establish a verifiable first-stage quotation foundation so one real internal quotation can be created, versioned, priced, approved, issued and queried through an API with traceable evidence.

| Field | Value |
|---|---|
| **Version** | v0.1.0 |
| **Status** | Candidate — Baseline Confirmed; not Committed |
| **Mission Owner** | Robin |
| **Product / Service Owner** | Jason Lin |
| **Target release / outcome date** | Missing — to be proposed after M1 walkthrough |
| **Risk level** | Candidate: High — commercial pricing, approval and sensitive cost data require cross-functional review |
| **Last updated** | 2026-07-17 (Asia/Singapore) |

## 1. Why

- **Value receiver:** STAR sales, presales, pricing, approval and operations users; merchants or customers receiving quotations; future CRM, Merchant Portal and partner integrations.
- **Problem / need:** quotation opportunities, pricing, cost, rules, approvals, versions and evidence do not yet have one verified Mission baseline. Manual or fragmented handling can create inconsistency, slow turnaround and weak auditability.
- **Why now:** SmartQuote is an active foundation initiative, but coordinated delivery cannot begin responsibly without named owners, a bounded first stage and agreed acceptance evidence.
- **Expected outcome:** one real internal quotation scenario completes end to end with retained versions, frozen pricing and channel-cost evidence, controlled approval and a documented API result.
- **Outcome measures:** first-scenario acceptance evidence below; quantitative baselines and improvement targets remain Missing and must be proposed after the walkthrough.

## 2. What

### In scope — Confirmed for the first stage

- minimum Merchant reference required for quotation;
- multiple Opportunities for one Merchant;
- Quote and Quote Version lifecycle, including V1/V2/V3 retention;
- pricing inputs required for the first accepted quotation scenario;
- frozen pricing-rule, rule and channel-cost snapshots for each generated Quote Version;
- configurable level, pricing and approval rules through Rule Center;
- minimum approval and permission flow for the first scenario;
- Quote issuance and retrieval;
- API-first contract and error handling for the accepted flow;
- audit evidence needed to explain quotation results;
- boundaries that do not prevent future Whitelabel and independent deployment.

### Out of scope — Confirmed for the first stage

- complete CRM, lead-management or sales-pipeline platform;
- complete Merchant Portal or customer self-service portal;
- Merchant Onboarding and full KYC/AML workflow;
- billing, settlement, ledger or payment execution;
- general-purpose Product Catalog beyond the accepted quotation need;
- general-purpose Rule, Pricing or Workflow platform for unrelated products;
- AI autonomous pricing, commercial approval or production-release authority;
- advanced BI and analytics platform;
- full legacy-system migration;
- complete post-quote implementation and go-live management;
- full multi-industry, multi-country or all-product expansion in this first stage.

### First acceptance and closure evidence — Confirmed

One real internal scenario must complete:

`Merchant → Opportunity → Quote → Quote Version → Pricing → Approval → Quote Issuance → API Query`

Evidence must verify:

- one Merchant with multiple Opportunities;
- Quote V1/V2/V3 version retention;
- pricing-rule and channel-cost snapshots;
- approval and permission boundaries;
- API contract and error handling;
- QA acceptance;
- Product Owner acceptance by Jason Lin;
- acceptance by a named business user representative, currently Missing.

Mission closure additionally requires release or operational evidence, monitoring, support readiness and explicit closure approval. Code or documentation merge alone is not completion.

## 3. Who

- **Mission Owner:** Robin — owns the bounded Mission outcome and M0–M4 progression; coordinates participants, scope, dependencies, blockers, risks, actions and evidence; escalates commercial, strategic, scope and resource decisions to Jason.
- **Product / Service Owner:** Jason Lin — owns SmartQuote product direction and long-term responsibility; approves scope priorities, commercial-rule direction, material product changes and Product Owner acceptance; participates in Mission closure.
- **Contributors:** Product, Architecture, Backend, Frontend, QA, DevOps/Operations, Sales, Presales, Pricing and other business participants as named during M1.
- **Approvers:** Jason for product direction and material commercial-rule changes; production-release and Mission-closure approvers remain Missing.
- **Reviewers / validators:** Architecture/technical authority, engineering representatives, QA, operations and the named business acceptance representative.
- **Operators / support:** Missing — to be named before M4.
- **Affected / informed parties:** quotation users, merchants/customers, support teams and future integrating systems.
- **External dependencies and contacts:** Unknown until the current system and source inventory is completed.
- **AI participation and human review boundary:** AI may assist with research, requirements, drafts, architecture options, code drafts, tests and documentation. Human owners must approve Mission scope, business rules, architecture, code, tests, release and closure. AI may not approve pricing, commercial exceptions, production release or Mission closure.

## 4. Now

- **Current state:** M0 baseline established. Leadership decisions, owners, first-stage boundaries, acceptance outcome, milestones and record location are Confirmed. M1 has not passed and formal implementation has not started.
- **Next three actions:**
  1. name the business acceptance representative and the remaining M1 role representatives;
  2. conduct the cross-functional M1 walkthrough using `WALKTHROUGH_PREPARATION.md`;
  3. record findings, resolve material gates and decide whether the Mission can become Committed and route to SmartQuote Delivery.
- **Blockers / dependencies:** named business acceptance representative; named Product, Architecture, Backend, Frontend, QA and DevOps/Operations representatives; target dates; authoritative inventory of existing SmartQuote product, architecture, code, prototype and test sources.
- **Open risks:** historical discussion being treated as approved scope; first stage expanding into a general platform; premature Whitelabel/deployment complexity; incorrect or unauthorized commercial rules; cost-data exposure; completion being claimed without business and operational evidence.
- **Decisions needed:** business acceptance representative; M1 participant names; proposed dates; production-release authority; Mission-closure authority; confirmed source and dependency owners.

## 5. Delivery and evidence

- **Release / operational path:** M0 baseline → M1 walkthrough → M2 first-stage design baseline → bounded implementation planning and delivery → M3 end-to-end demonstration → M4 delivery-readiness review. Formal implementation routing is prohibited before M1 passes and leadership authorizes commitment.
- **Quality and test evidence:** requirements traceability, business-rule examples, Quote Version and snapshot tests, permission and approval tests, API contract/error tests, regression evidence and QA acceptance.
- **Security / compliance / financial evidence:** access controls for pricing and cost data, approval authority, audit retention, commercial exception handling and financial-impact review; accountable reviewers remain Missing.
- **Customer or user evidence:** named internal business user acceptance is required; representative currently Missing.
- **Operational metrics / monitoring:** Candidate — API availability, quotation failure, rule-evaluation failure, approval delay, issuance failure and audit completeness.
- **Delayed outcome measurement owner and date:** Missing.
- **Learning recorded:** update this Mission Decision Log, Work Status and linked evidence after every milestone or material decision.

## Linked detail

- **Mission decisions:** [`DECISION_LOG.md`](DECISION_LOG.md)
- **Live status:** [`WORK_STATUS.md`](WORK_STATUS.md)
- **M1 preparation:** [`WALKTHROUGH_PREPARATION.md`](WALKTHROUGH_PREPARATION.md)
- **Product Delivery Mission intake:** [`../../16_ACTIVE_MISSION_INTAKE.md`](../../16_ACTIVE_MISSION_INTAKE.md)
- **Requirements / business rules:** Unverified / Not authoritative until located and reviewed.
- **Architecture / diagrams:** Unverified / Not authoritative until located and reviewed.
- **API / data contracts:** Missing.
- **Code / pull requests:** Unknown.
- **Test plans / evidence:** Missing.
- **Runbook / monitoring / rollback:** Missing.
- **Customer communication / feedback:** Missing.
