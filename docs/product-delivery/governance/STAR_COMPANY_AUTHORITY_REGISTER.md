# STAR Company Authority Register

| Field | Value |
|---|---|
| Status | Working register — appointments and acceptances incomplete |
| Governance basis | Company Minimum Control Baseline · Candidate Operational Baseline, GDEC-0013–GDEC-0020 |
| Work item | CP-07B · SmartQuote Named Authority Appointment and Explicit Acceptance |
| Leadership authorization | Approved by Jason Lin on 2026-08-02 |
| Scope | SmartQuote / PORT-003 / M001 appointment preparation only |
| Policy effect | None |
| Gate effect | None |
| Engineering Start effect | None |
| Last reviewed | 2026-08-02 |

## Use rules

- A role, title, Mission assignment, GitHub permission or system permission does not create Authority.
- An Authority becomes effective only after formal designation, explicit acceptance, conflict review, Source-of-Record completion, effective date, review trigger, replacement route, revocation route and required-access verification.
- Unaccepted records remain `Proposed — appointment pending`.
- This register does not pass M1 or Gate 2, grant Product Commitment, authorize Engineering Start, Delivery, Release, staging or production.
- Material Pricing Rule, Channel Cost, Financial Exception, Compliance Exception, Security Control, Access Elevation, Production Data Access and Production Release require four-eyes.

## SmartQuote Authority Register

| Authority ID | Authority | Proposed holder | Status | Exact scope | Accountability | Explicit exclusions | Independence / four-eyes | Required access | Effective date | Review trigger | Replacement route | Revocation route | Source of Record | Blocking stage |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| SQ-AUTH-001 | Product Authority re-binding | Jason Lin | Proposed — appointment pending | Product Intent, scope, priorities, business outcome, material product changes, Product Owner acceptance | Product direction and outcome | No Finance, Risk, Compliance, Architecture, Security or Release professional decisions | Independent professional review for pricing, cost, compliance, security and release matters | M001 product records; no automatic production access | Not effective | Product scope change, Commitment, Gate dispute | STAR Leadership | STAR Leadership | This register + M001 Authority Record | Before Product Commitment |
| SQ-AUTH-002 | Mission Coordination Authority re-binding | Robin Koh | Proposed — appointment pending | M1 organization, coordination, evidence, dependencies, blockers and readiness recommendation | Mission coordination integrity | Cannot change Product Intent, pass Gate, authorize Commitment, Delivery or Release | Cannot act as independent Business Acceptance Authority | M001 records and coordination tools | Not effective | M1, Mission-owner change, material blocker | Jason Lin / STAR Leadership | STAR Leadership | This register + M001 Authority Record | Before M1 |
| SQ-AUTH-003 | Engineering Authority | Ka Chen | Proposed — appointment pending | Engineering feasibility, implementation ownership, engineering quality and evidence | Engineering integrity | Cannot change Product Intent or approve own Release | Cannot be sole reviewer or Release Approver for own work | Company repository and dev/test environment after separate approval | Not effective | Engineering Start, major design change | Engineering leadership / STAR Leadership | Engineering leadership / STAR Leadership | This register + Engineering plan | Before Engineering Start; participate before M1 |
| SQ-AUTH-004 | QA Responsibility | Erica | Proposed — appointment pending | Test strategy, acceptance scenarios, test ownership and evidence | QA evidence integrity | Cannot grant Commitment or Release | Independent from implementation; QA + Product + Business acceptance | Requirements, test environment and CI evidence | Not effective | M1, DoD change, Release | QA leadership | QA leadership / STAR Leadership | This register + QA plan | Before M1 and Engineering Start |
| SQ-AUTH-005 | Operations Responsibility | Eric | Proposed — appointment pending | Environment, rollback, monitoring, support and operational evidence | Operational readiness | Cannot approve own access, Security Control, production deployment or Release | Operations + Engineering/QA; separate Release Authority | Approved dev/test environment only | Not effective | Environment creation, staging, release | Operations leadership | Operations leadership + access review | This register + Ops readiness record | Before Engineering Start / staging |
| SQ-AUTH-006 | Product Commitment Approver | Jason Lin | Proposed — appointment pending | Independent decision on bounded committed scope, resources, risks and stop conditions | Leadership commitment decision | Does not authorize Engineering Start or Release | Must rely on independent Architecture, Engineering, QA, Ops and professional evidence | M1, Gate 2, risk and resource evidence | Not effective | Commitment request or material scope/risk change | STAR Leadership | STAR Leadership | Commitment Decision Record | Before Product Commitment |
| SQ-AUTH-007 | Engineering Start Approver | Jason Lin | Proposed — appointment pending | Independent authorization for bounded engineering increment | Engineering Start decision | Does not authorize staging, production or scope expansion | Architecture + Engineering + QA + Operations readiness concurrence | Readiness evidence only; no automatic technical access | Not effective | Engineering Start request or restart | STAR Leadership | STAR Leadership / Stop Work decision | Engineering Start Decision Record | Before Engineering Start |
| SQ-AUTH-008 | Mission Closure Authority | Jason Lin | Proposed — appointment pending | Mission outcome, remaining risk, handover and closure decision | Mission closure disposition | Cannot bypass Business Acceptance, QA, Ops or unresolved risk | Business Acceptance + Mission recommendation + QA/Ops evidence | M0–M4 records | Not effective | M4 or termination proposal | STAR Leadership | STAR Leadership | Mission Closure Decision Record | Before Mission Closure |
| SQ-AUTH-009 | Business Acceptance Authority | Missing | Missing | Internal quotation outcome and business acceptance | Business acceptance truth | No Architecture, Pricing, Risk, Compliance or Release decisions | Independent from Mission coordination and implementation | Product pre-read and acceptance evidence | Missing | M1, M3, workflow change | Sales leadership | Product Authority / Sales leadership | M001 Authority Record | Before M1 |
| SQ-AUTH-010 | Architecture Authority | Missing | Missing | SoR, tenant, identity, permission, API, snapshot, repository, environment and deployment boundary | Architecture integrity | Cannot change Product Intent or automatically hold Engineering/Release Authority | Independent review of implementation it governs | Architecture records and read access | Missing | M1, Gate 2, architecture change | STAR Leadership / Architecture governance | STAR Leadership | Architecture SoR + M001 Authority Record | Before M1 / Gate 2 |
| SQ-AUTH-011 | Finance / Pricing Authority | Missing | Missing | Channel Cost, pricing, margin/floor ownership, approval threshold governance, FX/rounding/tax routing | Pricing and cost governance | No Product, Architecture or Release authority | Material Pricing and Channel Cost require four-eyes | Approved Finance source data | Missing | Pricing, cost or financial exception change | Finance leadership | Finance leadership / STAR Leadership | Finance SoR + M001 Authority Record | Before M1 / Gate 2 |
| SQ-AUTH-012 | Risk Review Responsibility | Missing | Missing | Risk classification, hard-block review, exceptions and escalation | Independent risk review | No Product, Compliance, Security or Leadership decisions | Requester cannot be sole Risk Acceptor | Approved risk evidence | Missing | Risk, exception, real data, staging/production | Risk leadership | Risk leadership / STAR Leadership | Risk SoR + M001 Authority Record | Route before M1; substantive before Gate 2 |
| SQ-AUTH-013 | Compliance Review Responsibility | Missing | Missing | Prohibited activities, regulatory hard blocks, retention, data restrictions and exceptions | Compliance review correctness | No Product, Pricing or Architecture decisions | Product/Engineering cannot approve own exception | Approved Compliance evidence | Missing | Regulatory scope, real data, exception | Compliance leadership | Compliance leadership / STAR Leadership | Compliance SoR + M001 Authority Record | Route before M1; substantive before Gate 2 |
| SQ-AUTH-014 | Security Review Responsibility | Missing | Missing | Identity, permission, tenant isolation, encryption, secrets and audit integrity | Security review integrity | No automatic Engineering, Ops or Release authority | Admin/developer cannot approve own elevation or control | Security evidence; production access separately approved | Missing | Gate 2, environment, access, staging/production | Security leadership | Security leadership / STAR Leadership | Security SoR + M001 Authority Record | Before Gate 2 / staging |
| SQ-AUTH-015 | Release Authority | Missing | Missing | Staging and production release authorization | Release decision and rollback readiness | Cannot bypass Critical Security Risk or change Product Intent | Developer cannot be sole reviewer and Release Approver | Release evidence; deployment permission separate | Missing | First staging, first production, material release | STAR Leadership / Ops governance | STAR Leadership / Emergency route | Release Decision Record | Before staging / production |
| SQ-AUTH-016 | Sales Representative | Missing | Missing | Current quotation facts and Sales-user perspective | Accuracy of current-process evidence | Cannot approve own Pricing exception | Separate Finance approval for exceptions | Product pre-read and process-observation materials | Missing | M1 and workflow change | Sales leadership | Sales leadership | M001 Authority Record | Before M1 |
| SQ-AUTH-017 | Channel Cost Accountable Contact | Missing | Missing | Route Channel Cost owner, SoR and maintenance process | Ownership routing accuracy | Cannot self-approve material Channel Cost changes | Channel Cost requires four-eyes | Approved Channel Cost source access only | Missing | Channel Cost or pricing change | Finance / Channel leadership | Finance / Channel leadership | Finance SoR + M001 Authority Record | Before Gate 2 |

## Candidate-identification constraint

No missing Authority has been assigned a person. Candidate identification requires evidence of professional competence, independence, exact scope, access need and explicit acceptance. Historical tasks, reporting lines or technical permissions are insufficient.

## Current control state

```text
Formal appointments: Not effective
Explicit acceptance: Not yet obtained
M1: Hold / Not Passed
Gate 2: Hold / Not Passed
Product Commitment: Not Granted
Engineering Start: Not Authorized
Product-code repository creation: Not Authorized
Coding: Not Authorized
Real-data use: Not Authorized
Staging / Production: Not Authorized
```
