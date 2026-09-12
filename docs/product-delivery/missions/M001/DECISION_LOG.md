# M001 · SmartQuote Foundation — Decision Log

| Field | Value |
|---|---|
| **Version / status** | v0.2.0 — Active Mission-level decisions |
| **Mission status** | Candidate — Baseline Confirmed; not Committed |
| **Mission Owner** | Robin |
| **Product / Service Owner** | Jason Lin |
| **Last consolidated** | 2026-09-12 (Asia/Singapore) |
| **Authoritative source** | This path in Draft PR #1 on `agent/star-os-product-delivery-baseline` |

## Use rules

- Entries are append-only.
- Corrections require a new Decision ID that explicitly supersedes an earlier entry.
- Unsupported historical completion or freeze claims are `Unverified / Not authoritative`; they are not `Superseded` without an explicit authoritative supersession record.
- These decisions establish the Mission baseline but do not authorize formal implementation.

## Confirmed decisions

| ID | Decision | Scope | Basis |
|---|---|---|---|
| **M001-DEC-001** | Robin is the Mission Owner. | M001 | Leadership Dispatch DSP-003-003 |
| **M001-DEC-002** | Jason Lin is the Product / Service Owner. | M001 | Leadership Dispatch DSP-003-003 |
| **M001-DEC-003** | The first-stage In Scope and Out of Scope boundaries in `MISSION_BRIEF.md` are approved. | M001 first stage | Leadership Dispatch DSP-003-003 |
| **M001-DEC-004** | The first acceptance outcome is one real internal flow: Merchant → Opportunity → Quote → Quote Version → Pricing → Approval → Quote Issuance → API Query. | M001 first acceptance | Leadership Dispatch DSP-003-003 |
| **M001-DEC-005** | Acceptance must verify multiple Opportunities per Merchant, Quote V1/V2/V3 retention, pricing-rule and channel-cost snapshots, approval and permission boundaries, API contract/error handling, QA acceptance, Product Owner acceptance and business-user acceptance. | M001 first acceptance | Leadership Dispatch DSP-003-003 |
| **M001-DEC-006** | M001 milestones are M0 Baseline Confirmed, M1 Cross-functional Walkthrough Passed, M2 First-stage Design Baseline Approved, M3 First End-to-End Demonstration Accepted and M4 Delivery Readiness Approved. | M001 lifecycle | Leadership Dispatch DSP-003-003 |
| **M001-DEC-007** | The authoritative Mission record location is `STAR-SAAS/star-architecture`, Draft PR #1, branch `agent/star-os-product-delivery-baseline`. | M001 records | Leadership Dispatch DSP-003-003 |
| **M001-DEC-008** | Robin owns the bounded outcome and M0–M4 progression, coordinates cross-functional participants and evidence, and escalates unresolved commercial, strategic, scope and resource decisions to Jason. Robin does not independently approve product direction, commercial pricing rules, production release or Mission closure. | M001 responsibility | Leadership Dispatch DSP-003-003 |
| **M001-DEC-009** | Jason owns SmartQuote product direction and enduring responsibility, approves scope priorities, commercial-rule direction, material product changes and Product Owner acceptance, and participates in Mission closure. | M001 responsibility | Leadership Dispatch DSP-003-003 |
| **M001-DEC-010** | After this record set is written, Mission status may be `Candidate — Baseline Confirmed`. It must not become `Committed` until M1 passes. | M001 status | Leadership Dispatch DSP-003-003 |
| **M001-DEC-011** | Formal implementation must not be routed to SmartQuote Delivery before M1 passes and commitment is authorized. | M001 routing | Leadership Dispatch DSP-003-003 |
| **M001-DEC-012** | A named business acceptance representative is required before final business acceptance and remains Missing. | M001 acceptance gate | Leadership Dispatch DSP-003-003 |
| **M001-DEC-013** | One Merchant may have multiple Opportunities. | SmartQuote product constraint | Previously confirmed product decision reaffirmed in DSP-003-002/003 context |
| **M001-DEC-014** | Quote supports retained versions such as V1, V2 and V3. | SmartQuote product constraint | Previously confirmed product decision reaffirmed in DSP-003-002/003 context |
| **M001-DEC-015** | A generated Quote Version freezes the channel-cost and rule snapshot used at generation time. | SmartQuote product constraint | Previously confirmed product decision reaffirmed in DSP-003-002/003 context |
| **M001-DEC-016** | Level, pricing and approval rules are configurable through Rule Center. | SmartQuote product constraint | Previously confirmed product decision reaffirmed in DSP-003-002/003 context |
| **M001-DEC-017** | SmartQuote is API-first for future CRM, Merchant Portal and partner integration. | SmartQuote product constraint | Previously confirmed product decision reaffirmed in DSP-003-002/003 context |
| **M001-DEC-018** | SmartQuote must eventually support Whitelabel and independent deployment; this is a future product constraint, not permission to over-expand the first stage. | SmartQuote product constraint | Previously confirmed product decision reaffirmed in DSP-003-002/003 context |
| **M001-DEC-019** | Unsupported historical completion or freeze claims are classified as `Unverified / Not authoritative`; `Superseded` requires an explicit authoritative supersession record. | M001 evidence classification | Leadership Dispatch DSP-003-003 |
| **M001-DEC-020** | `STAR-SAAS/smartquote` is the approved independent SmartQuote product engineering repository. `STAR-SAAS/star-architecture` remains the M001 Mission/Gate/Authority working SoR; `STAR-SAAS/star-ai-governance` remains the company governance/SAIG/SAES SoR; `smartquote` becomes the product/engineering SoR only as specific work is authorized. Repository creation does not pass M1 or Gate 2, commit M001, make any Authority effective, grant Product Commitment, authorize Engineering Start, or authorize Release. | M001 repository and SoR boundary | Leadership decision 2026-09-12; `M001-REPO-BINDING-001` |

## Open decision gates

- Named business acceptance representative.
- Named M1 representatives for Product, Architecture, Backend, Frontend, QA and DevOps/Operations.
- Target milestone dates.
- Production-release authority.
- Mission-closure authority.
- Security, compliance and financial reviewers required for pricing, cost and approval evidence.
- Effective Engineering Authority and L2 engineering-profile acceptance before material implementation.
