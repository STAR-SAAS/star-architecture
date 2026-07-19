# PDAP Architecture Readiness Matrix

| Program / Product | Current phase / Gate | Current state | Freshness | Target start | Accountable owner | Primary executor | Specialist required | Current forecast | Blocking decision | Next action |
|---|---|---|---|---|---|---|---|---|---|---|
| PDAP | Phase 2–4 preparation completed | Gate 1–3 preparation package ready for publication; no Gate passed | Current | N/A | Jason Lin | Jason Lin + approved AI | None now | On target for preparation | publication and disposition remain | publish package, then Gate 1 internal disposition |
| Shared Foundation | Phase 2 / Gate 1 | Recovery required recommendation; engineering not started | Current / partially Unverified | 2026-07-27 | Jason Lin | Jason Lin + approved AI | Ka Chen and Eric are later candidates only | At risk | bootstrap, owner, environment, CI/test, secrets and rollback | DSP-001-027 Gate 1 internal disposition |
| SmartQuote | Phase 3 / Gate 2 | Conditional pass candidate recommendation only; M1 not passed; M001 not Committed; Delivery not started | Current | 2026-08-03 | Jason Lin | Jason Lin + approved AI | only if a specific feasibility question triggers | At risk | SoR, channel-cost owner, repository/environment, security/test, M1 and Commitment | close Gate 2 conditions |
| GateHub | Phase 4 / Gate 3 | Recovery required recommendation; Candidate authority; Delivery not started | Current Candidate / Unverified implementation | 2026-08-10 | Jason Lin | Jason Lin + approved AI | only if a specific professional question triggers | At risk | authority, Compliance source, repository/provider scenario and restricted-data evidence | recover Gate 3 evidence |
| Cross-product Review | Preview only / Gate 4 not started | conflict candidates identified; Merchant Identity and channel-cost require later decision | Current coordination state | Before relevant Commitment | Jason Lin | Jason Lin + approved AI | only if triggered | Not yet forecast | ownership and interface conflicts | formal Gate 4 after product packages mature |

## Approved operating inputs

- Shared Foundation is engineering-foundation-first; product capabilities remain product-owned until stable reuse is proven.
- Merchant ownership is layered; Merchant Identity remains for Gate 4.
- Identity/Tenant/Security minimum boundaries are design inputs, not final architecture.
- `STAR-SAAS/star-platform` remains Candidate and not engineering-ready.
- GateHub first stage excludes payment routing, transaction execution, settlement and ledger.
- Reusable channel-cost source ownership must close before actual Gate 2 disposition.
- AA-01 through AA-04 are approved temporary assumptions.
- AA-05 through AA-09 remain Candidate.

## Update rules

- Recommendations do not equal Gate passage.
- Target dates are not automatic authorization.
- Missing or Unverified evidence remains explicit.
- Every blocker records owner, evidence, closure date and recovery action.
- Approved Assumptions retain scope, risk, trigger, expiry and reversal path.