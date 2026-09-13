# M001 · SmartQuote Foundation — Active Decisions

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Confirmed runtime projection; not a replacement for the full Decision Log |
| **Scope** | `PORT-003 · Mission-001 · SmartQuote Foundation` |
| **Mission state** | Candidate — Baseline Confirmed; not Committed |
| **Mission Owner** | Robin |
| **Product / Service Owner** | Jason Lin |
| **Authoritative source** | `DECISION_LOG.md` on `agent/star-os-product-delivery-baseline` |
| **Source snapshot commit** | `fb66ee5b462cedc48e56ac2fb61f3f07682b70e9` |
| **Source Decision Log blob** | `4615bf910e60e09aed15841ac41cf606d6d1c915` |
| **Last verified** | 2026-07-17T19:10:39+08:00 |

## Runtime use

This file is the concise required payload for the SWS Pilot Package B resume test. It contains only active confirmed M001 decisions needed to reconstruct the Mission safely. The full append-only history remains in `DECISION_LOG.md`.

## Identity and authority

- **M001-DEC-001:** Robin is the Mission Owner.
- **M001-DEC-002:** Jason Lin is the Product / Service Owner.
- **M001-DEC-007:** The authoritative Mission record is in `STAR-SAAS/star-architecture`, Draft PR #1, branch `agent/star-os-product-delivery-baseline`.
- **M001-DEC-008:** Robin owns the bounded outcome and M0–M4 progression, coordinates participants and evidence, and escalates unresolved commercial, strategic, scope and resource decisions to Jason. Robin does not independently approve product direction, commercial pricing rules, production release or Mission closure.
- **M001-DEC-009:** Jason owns SmartQuote product direction and enduring responsibility, approves scope priorities, commercial-rule direction, material product changes and Product Owner acceptance, and participates in Mission closure.

## First-stage boundary and acceptance

- **M001-DEC-003:** The first-stage In Scope and Out of Scope boundaries in `MISSION_BRIEF.md` are approved.
- **M001-DEC-004:** The first acceptance outcome is one real internal flow: `Merchant → Opportunity → Quote → Quote Version → Pricing → Approval → Quote Issuance → API Query`.
- **M001-DEC-005:** Acceptance must verify multiple Opportunities per Merchant, Quote V1/V2/V3 retention, pricing-rule and channel-cost snapshots, approval and permission boundaries, API contract and error handling, QA acceptance, Product Owner acceptance and business-user acceptance.
- **M001-DEC-006:** Milestones are M0 Baseline Confirmed, M1 Cross-functional Walkthrough Passed, M2 First-stage Design Baseline Approved, M3 First End-to-End Demonstration Accepted and M4 Delivery Readiness Approved.

## Confirmed SmartQuote constraints

- **M001-DEC-013:** One Merchant may have multiple Opportunities.
- **M001-DEC-014:** Quote supports retained versions such as V1, V2 and V3.
- **M001-DEC-015:** A generated Quote Version freezes the channel-cost and rule snapshot used at generation time.
- **M001-DEC-016:** Level, pricing and approval rules are configurable through Rule Center.
- **M001-DEC-017:** SmartQuote is API-first for future CRM, Merchant Portal and partner integration.
- **M001-DEC-018:** SmartQuote must eventually support Whitelabel and independent deployment; this future constraint does not expand the approved first stage.

## Independent gates and prohibitions

- **M001-DEC-010:** M001 must not become `Committed` until M1 passes.
- **M001-DEC-011:** Formal implementation must not be routed to SmartQuote Delivery before M1 passes and leadership authorizes commitment.
- **M001-DEC-012:** A named business acceptance representative is required before final business acceptance and remains Missing.
- Package B completion is context-recovery evidence only. It does not pass M1, authorize commitment, approve production release or start SmartQuote Delivery.

## Evidence classification

- **M001-DEC-019:** Unsupported historical completion or freeze claims are `Unverified / Not authoritative`. `Superseded` requires an explicit authoritative supersession record.

## Remaining Missing — not decisions

- named business acceptance representative;
- named Product, Architecture, Backend, Frontend, QA and DevOps/Operations M1 representatives;
- target milestone dates;
- production-release authority;
- Mission-closure authority;
- Security, Compliance and Finance review responsibilities;
- authoritative inventory of existing SmartQuote product, architecture, code, prototype and test sources.
