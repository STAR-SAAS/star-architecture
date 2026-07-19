# PDAP Phase 1 Decision, Blocker and Report Back

## Status

- Dispatch: `DSP-001-023`
- Result: Completed read-only analysis; leadership decisions approved
- Gate 1: Not passed
- Shared Foundation engineering: Not started
- M1: Not passed
- M001: Not Committed
- SmartQuote Delivery: Not started
- GateHub Delivery: Not started

## Approved Assumptions

### AA-01 — Shared Foundation bounded start

- Owner: Jason Lin
- Scope: Shared Foundation
- Assumption: establish minimum engineering controls and stable shared foundations, not a broad business platform.
- Risk: module boundaries may later change.
- Trigger: first proposed shared business capability.
- Expiry: 2026-07-31 or Gate 1 disposition, whichever comes first.
- Reversal: keep capability in the product repository.

### AA-02 — Product ownership by default

- Owner: Jason Lin
- Scope: SmartQuote, GateHub and Shared Foundation
- Assumption: capabilities remain product-owned until stable cross-product reuse is evidenced.
- Risk: limited temporary duplication.
- Trigger: second product demonstrates the same stable need.
- Expiry: 2026-07-31 or Cross-product Review.
- Reversal: extract through ADR/RFC.

### AA-03 — SmartQuote internal API before external platform selection

- Owner: Jason Lin
- Scope: SmartQuote
- Assumption: define an internal API contract without waiting for CRM, Merchant Portal or partner-platform technology choices.
- Risk: later adapter or version evolution.
- Trigger: first external consumer.
- Expiry: 2026-07-31 or Gate 2 disposition.
- Reversal: versioning, adapter or contract migration.

### AA-04 — GateHub independent authority

- Owner: Jason Lin
- Scope: GateHub
- Assumption: establish GateHub business and architecture authority independently of SmartQuote.
- Risk: additional initial work.
- Trigger: GateHub minimum architecture package.
- Expiry: 2026-07-31 or Gate 3 disposition.
- Reversal: approve shared decisions during Cross-product Review.

AA-05 technology-neutral observability signals and AA-06 tool-neutral CI controls remain Candidate and are not approved for use.

## Blocker candidates and recovery

| ID | Candidate | Class | Owner | Target closure | Recovery |
|---|---|---|---|---|---|
| B-01 | Merchant ownership | Core data ownership | Jason Lin | 2026-07-24 | separate Identity, Commercial Profile, Onboarding/KYC, Quote Reference and Operational Account |
| B-02 | Identity / Tenant boundary | Identity / Tenant / Security | Jason Lin | 2026-07-24 | use approved minimum boundary without selecting final technology |
| B-03 | Shared Foundation engineering owner | Engineering-start authority | Jason Lin | before engineering start | confirm candidate after temporary review-only window; no current task assignment |
| B-04 | GateHub authority | Product authority | Jason Lin | 2026-07-26 | approve bounded Candidate definition, scope and exclusions before architecture disposition |
| B-05 | SmartQuote pricing and channel-cost disposition | Security / material commercial risk | Jason Lin | before Gate 2 disposition | Confidential classification, least privilege, immutable snapshot and audit as default candidates |

## ADR and RFC backlog

Priority ADRs:

1. Shared versus product capability ownership.
2. Merchant identity and master-data ownership.
3. Tenant context and isolation.
4. Authentication versus product authorization.
5. SmartQuote Quote/Quote Version system of record.
6. Rule Center ownership.
7. Channel-cost source versus Quote snapshot.
8. GateHub onboarding and KYC boundary.
9. Connector ownership and lifecycle.
10. Audit-event ownership and shared envelope.

Priority RFCs:

1. Shared Foundation repository/module structure.
2. Environment and promotion model.
3. Git/PR/CI controls.
4. Secrets and configuration.
5. Observability and audit.
6. Deployment and rollback.
7. API versioning, errors and correlation.
8. Testing baseline.
9. Whitelabel and independent-deployment constraints.
10. Bank/PSP connector contract.

## Forecast

| Target | Current forecast | Conditions |
|---|---|---|
| Shared Foundation — 2026-07-27 | At risk | Gate 1 disposition, repository/environment/CI/test baseline and owner requirement |
| SmartQuote — 2026-08-03 | At risk but recoverable | minimum architecture package, Gate 2, Cross-product Review, M1 and separate Commitment |
| GateHub — 2026-08-10 | At risk | Candidate authority confirmation before architecture package and Gate 3 disposition |

These target dates remain approved targets, not automatic authorization.

## Leadership decisions recorded

Leadership approved:

- engineering-foundation-first Shared Foundation boundary;
- Merchant layered ownership candidates;
- Identity/Tenant/Security minimum boundary;
- `STAR-SAAS/star-platform` as Candidate Shared Foundation repository;
- GateHub Candidate authority baseline;
- AA-01 through AA-04;
- target dates of 2026-07-27, 2026-08-03 and 2026-08-10;
- Ka Chen as Shared Foundation application engineering owner candidate;
- Eric as platform/infrastructure/operations owner candidate.

Candidate roles are not current task assignments and do not authorize engineering.

## Temporary participation rule

Through 2026-07-26, Jason Lin with approved AI capabilities remains the executor. Dorden, Robin and Allen receive no execution task and review only consolidated conclusions when requested.

## Self-review

No technology stack, product architecture, Gate passage, M1, Product Commitment, engineering start or Delivery start is approved by this record.