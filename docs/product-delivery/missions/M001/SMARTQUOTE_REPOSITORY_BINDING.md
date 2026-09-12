# M001 · SmartQuote Repository Binding

| Field | Value |
|---|---|
| Record ID | `M001-REPO-BINDING-001` |
| Status | Candidate — repository binding prepared; no Gate or Engineering effect |
| Mission | `M001 · SmartQuote Foundation` |
| Product repository | `STAR-SAAS/smartquote` |
| Product repository state | Created; Governance Bootstrap Draft PR #1 open / draft / unmerged |
| Governance bootstrap Head | `304055ff5b22045cf93b7e28f20784f3d7d0817b` |
| Governance bootstrap Tree | `de05cfd3ea29fed0c06bb9f240b5febd77c18828` |
| Mission / Gate SoR | `STAR-SAAS/star-architecture` |
| Company governance SoR | `STAR-SAAS/star-ai-governance` |
| Prepared on | 2026-09-12 |

## Binding decision

`STAR-SAAS/smartquote` is the approved independent SmartQuote product engineering repository. Repository creation supersedes only the earlier historical fact that no SmartQuote product repository existed. It does not supersede or silently modify M001 scope, Gate state, Authority state, Product Commitment, Engineering Start or Release controls.

## Repository responsibility boundary

### `STAR-SAAS/star-architecture`

Remains the working Source of Record for:

- M001 Mission purpose, scope, exclusions and lifecycle;
- M1 and Gate 2 decisions;
- Product Commitment and Engineering Start decisions;
- company/cross-project architecture decisions;
- M001 Authority appointment and explicit-acceptance records.

### `STAR-SAAS/star-ai-governance`

Remains the Source of Record for:

- STAR Company Governance Baseline;
- SAIG and SAES standards;
- Safety Foundation and governance adoption / upgrade controls.

### `STAR-SAAS/smartquote`

May become the Source of Record, when separately authorized, for:

- detailed SmartQuote product requirements;
- domain and lifecycle specifications;
- product ADRs;
- API contracts;
- data model and migrations;
- frontend/backend implementation;
- tests, CI and engineering evidence;
- repository-specific release evidence.

The product repository may not self-pass Mission/company gates or redefine professional Authority recorded elsewhere.

## Authority / Gate rebinding

Current canonical Authority references remain in Draft PR #19 and retain their existing proposal states:

- `SQ-AUTH-003` — Engineering Authority — Ka Chen — `Proposed — appointment pending`;
- `SQ-AUTH-006` — Product Commitment Approver — Jason Lin — `Proposed — appointment pending`;
- `SQ-AUTH-007` — Engineering Start Approver — Jason Lin — `Proposed — appointment pending`;
- `SQ-AUTH-015` — Release Authority — Missing.

Repository ownership or GitHub access does not make any of these Authorities effective.

Current Gate state remains:

- M1: Hold / Not Passed;
- Gate 2: Hold / Not Passed;
- Product Commitment: Not Granted;
- Engineering Start: Not Authorized;
- Formal Delivery: Not Started;
- Production Release: Not Authorized.

## Bootstrap dependency

SmartQuote Governance Bootstrap PR #1 must be human-merged and post-merge Commit/Tree/Blob readback must pass before the product repository can be recorded as `Installed / Report-only` for governance inheritance.

This repository-binding record does not require PR #19 to be rewritten and does not invalidate its exact Authority proposal object. PR #19 remains a separate Draft Authority package pending explicit acceptance, conflict resolution and a later effectiveness decision.

## Non-effects

This record does not:

- pass M1 or Gate 2;
- commit M001;
- make any Authority effective;
- authorize product code, build/runtime dependencies, database migrations or environment creation;
- authorize real merchant/customer/channel-cost data;
- authorize Connector, credential, staging, production or Release activity;
- authorize AI merge.
