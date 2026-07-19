# PDAP Architecture Readiness Matrix

| Program / Product | Current phase / Gate | Current state | Freshness | Target start | Accountable owner | Primary executor | Specialist required | Current forecast | Blocking decision | Next action |
|---|---|---|---|---|---|---|---|---|---|---|
| PDAP | Phase 1 completed / Gate 1 preparation | Phase 0 evidence and Phase 1 shared constraints completed; no Gate declared passed | Current | Phase 0 started 2026-07-20 | Jason Lin | Jason Lin + approved AI | No current task | On target for preparation | None confirmed beyond recorded blocker candidates | publish Phase 0/1 authority and continue Gate evidence |
| Shared Foundation | Phase 2 preparation / Gate 1 | Candidate boundary and repository disposition approved; engineering readiness not verified | Current / partially Unverified | 2026-07-27 | Jason Lin | Jason Lin + approved AI | Ka Chen and Eric are later candidates only | At risk | repository/environment/CI/test baseline and post-start owner | prepare minimum engineering-start evidence; no engineering start |
| SmartQuote | Phase 3 preparation / Gate 2 | Mission boundary current; Architecture Gate not passed; M1 not passed; M001 not Committed; Delivery not started | Current | 2026-08-03 | Jason Lin | Jason Lin + approved AI | only if specific feasibility question triggers | At risk but recoverable | architecture package, sensitive-data disposition, repository/environment, M1 and Commitment | complete minimum architecture package |
| GateHub | Candidate authority baseline / Gate 3 preparation | Candidate business definition, scope and exclusions approved; architecture evidence Missing | Current Candidate / Unverified implementation | 2026-08-10 | Jason Lin | Jason Lin + approved AI | only if specific feasibility question triggers | At risk | architecture package, ownership and implementation evidence | develop minimum architecture package without inheriting SmartQuote architecture |
| Cross-product Review | Not started / Gate 4 | Candidate dependency and ownership conflicts identified | Current coordination state | Before relevant Commitment | Jason Lin | Jason Lin + approved AI | only if triggered | Not yet forecast | Merchant ownership, Identity/Tenant/Security and connector ownership | compare after shared and product packages exist |

## Approved operating inputs

- Shared Foundation is engineering-foundation-first; shared business capabilities require demonstrated stable reuse.
- Merchant ownership is layered across Identity, Commercial Profile, Onboarding/KYC, Quote Reference and Operational Account.
- Identity/Tenant/Security minimum boundaries are approved design inputs, not final architecture.
- `STAR-SAAS/star-platform` is a Candidate Shared Foundation repository; engineering start is not authorized.
- GateHub has a Candidate authority baseline, not an approved product architecture.
- AA-01 through AA-04 are approved until their stated expiry or Gate disposition.
- AA-05 and AA-06 remain Candidate.

## Update rules

- `Freshness` describes evidence freshness, not Gate passage.
- Target dates are not automatic approval.
- Missing or Unverified evidence stays explicit.
- Every blocker records owner, due date, recovery action and authoritative source.
- Approved Assumptions record scope, risk, owner, validation trigger, expiry/review date and reversal path.