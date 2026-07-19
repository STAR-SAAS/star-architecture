# PDAP Blocker, Recovery and Schedule Register

## Blockers

| ID | Gate | Blocker | Class | Owner | Evidence required | Closure target | Recovery | Current disposition |
|---|---|---|---|---|---|---|---|---|
| B-01 | Gate 1 | `star-platform` empty | Technical readiness | Jason Lin | approved and implemented bounded bootstrap | disposition by 2026-07-24; implementation before start | preparation only | remains open; documentation does not close it |
| B-02 | Gate 1 | engineering owner not assigned | Authority | Jason Lin | accepted application and platform/operations ownership | before Gate 1 passage and engineering start | hold actual start | remains open; not safely deferrable |
| B-03 | Gate 1 | environment/CI/tests absent | Technical/recovery | Jason Lin pending named owners | executable non-production environment, build, checks and tests | before first engineering merge | restrict to preparation | remains open; AA-06 covers tool choice only |
| B-04 | Gate 1 | secrets/deployment/rollback absent | Security/recovery | Jason Lin pending platform/operations owner | secrets boundary, deployment evidence and rollback/recovery | before engineering start | no production access | remains open; vendor/topology may be deferred only |
| B-05 | Gate 2 | Merchant/channel-cost source ownership unresolved | Core data ownership | Jason Lin | ownership disposition | 2026-07-29 | stable references and frozen snapshots | open |
| B-06 | Gate 2 | repository/environment Missing | Technical readiness | Jason Lin | approved repository/environment | 2026-07-29 | architecture-only work | open |
| B-07 | Gate 2 | security/data disposition unvalidated | Security/material risk | Jason Lin | classification/access review | 2026-07-31 | treat cost/pricing as Confidential | open |
| B-08 | Gate 3 | authority/package remains Candidate | Product authority | Jason Lin | leadership disposition | 2026-07-26 | no product architecture approval | open |
| B-09 | Gate 3 | Compliance source Missing | Legal/compliance | Jason Lin | authoritative professional source | 2026-08-04 | exclude final KYC decisions | open |
| B-10 | Gate 3 | repository/provider scenario Missing | Technical readiness | Jason Lin | one bounded provider scenario | 2026-08-04 | design-only package | open |
| B-11 | Gate 4 | reusable channel-cost owner Missing | Cross-product/data | Jason Lin | system-of-record decision | 2026-07-31 | SmartQuote stores immutable snapshot | open |

## Specialist triggers

No specialist is required now. After 2026-07-26, two concentrated validations may be prepared: application engineering feasibility for the bounded repository/build/test/check interface, and platform/operations feasibility for non-production environment, secrets, deployment and rollback. This record assigns no task and does not establish final owners.

## Schedule

| Target | Forecast | Conditions |
|---|---|---|
| Shared Foundation engineering — 2026-07-27 | At risk; retained conditionally | Gate 1 passage, separate engineering authorization, actual owners, implemented bounded bootstrap, non-production environment, build/test/check path, secrets and recovery evidence |
| SmartQuote formal development — 2026-08-03 | At risk | Gate 2 disposition, SoR closure, repository/environment, API/data/security/test evidence, M1 and Commitment |
| GateHub formal development — 2026-08-10 | At risk | authority disposition, Compliance source, bounded provider scenario, repository/environment and Gate 3/4 disposition |

The 2026-07-24 date is a disposition cutoff, not automatic blocker closure. If required evidence is not available, the 2026-07-27 target must be reforecast. A 2026-07-29 to 2026-07-31 fallback is planning only and is not an approved target.

## Recovery principles

Close only applicable Gate blockers with actual evidence. Use approved assumptions for reversible tool choices, not for missing ownership, security or executable controls. Do not expand first slices, build broad platforms, start product implementation or treat documentation completion as readiness.