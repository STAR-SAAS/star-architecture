# PDAP Blocker, Recovery and Schedule Register

## Blockers

| ID | Gate | Blocker | Class | Owner | Evidence required | Closure target | Recovery |
|---|---|---|---|---|---|---|---|
| B-01 | Gate 1 | `star-platform` empty | Technical readiness | Jason Lin | approved bounded bootstrap | 2026-07-24 | preparation only |
| B-02 | Gate 1 | engineering owner not assigned | Authority | Jason Lin | explicit post-start ownership | before engineering start | hold actual start |
| B-03 | Gate 1 | environment/CI/tests absent | Technical/recovery | Jason Lin | minimum executable controls | before first engineering merge | restrict to preparation |
| B-04 | Gate 1 | secrets/deployment/rollback absent | Security/recovery | Jason Lin | minimum control evidence | before engineering start | no production access |
| B-05 | Gate 2 | Merchant/channel-cost source ownership unresolved | Core data ownership | Jason Lin | ownership disposition | 2026-07-29 | stable references and frozen snapshots |
| B-06 | Gate 2 | repository/environment Missing | Technical readiness | Jason Lin | approved repository/environment | 2026-07-29 | architecture-only work |
| B-07 | Gate 2 | security/data disposition unvalidated | Security/material risk | Jason Lin | classification/access review | 2026-07-31 | treat cost/pricing as Confidential |
| B-08 | Gate 3 | authority/package remains Candidate | Product authority | Jason Lin | leadership disposition | 2026-07-26 | no product architecture approval |
| B-09 | Gate 3 | Compliance source Missing | Legal/compliance | Jason Lin | authoritative professional source | 2026-08-04 | exclude final KYC decisions |
| B-10 | Gate 3 | repository/provider scenario Missing | Technical readiness | Jason Lin | one bounded provider scenario | 2026-08-04 | design-only package |
| B-11 | Gate 4 | reusable channel-cost owner Missing | Cross-product/data | Jason Lin | system-of-record decision | 2026-07-31 | SmartQuote stores immutable snapshot |

## Specialist triggers

No specialist is required now. Future triggers include Security/Architecture for Identity/Tenant feasibility, application engineering for maintainable bootstrap, DevOps/Operations for executable environment and rollback, Compliance/Legal for KYC retention/residency, commercial/security review for pricing access and QA for first-slice test feasibility.

The temporary founder-led window assigns no work to Dorden, Robin, Allen, Ka Chen or Eric.

## Schedule

| Target | Forecast | Conditions |
|---|---|---|
| Shared Foundation engineering — 2026-07-27 | At risk | Gate 1 disposition, bounded bootstrap, named owner, non-production environment, build/test/check path, secrets and rollback direction |
| SmartQuote formal development — 2026-08-03 | At risk | Gate 2 disposition, SoR closure, repository/environment, API/data/security/test evidence, M1 and Commitment |
| GateHub formal development — 2026-08-10 | At risk | authority disposition, Compliance source, bounded provider scenario, repository/environment and Gate 3/4 disposition |

Target dates are not authorization. If Gate 1 is not dispositioned by 2026-07-24, the 2026-07-27 engineering target must be reforecast.

## Recovery principles

Close only applicable Gate blockers. Use approved assumptions for reversible matters. Do not expand first slices, build broad platforms, start product implementation or treat documentation completion as readiness.