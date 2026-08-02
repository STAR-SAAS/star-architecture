# M001 · SmartQuote Authority Record

| Field | Value |
|---|---|
| Work item | CP-07B · SmartQuote Named Authority Appointment and Explicit Acceptance |
| Leadership authorization | Approved by Jason Lin on 2026-08-02 |
| Mission | PORT-003 · M001 · SmartQuote Foundation |
| Mission status | Candidate — Baseline Confirmed; not Committed |
| Record status | Appointment proposals recorded; explicit acceptance pending |
| M1 | Hold / Not Passed |
| Gate 2 | Hold / Not Passed |
| Product Commitment | Not Granted |
| Engineering Start | Not Authorized |
| Last reviewed | 2026-08-02 |

## Purpose

Record SmartQuote Authority appointment proposals, explicit-acceptance requirements, conflicts, professional routing and M1-readiness facts without creating effective appointments or authorizing Engineering.

## Approved appointment proposals

| Authority ID | Authority | Proposed holder | Current status | Existing record basis | Acceptance required |
|---|---|---|---|---|---|
| SQ-AUTH-001 | Product Authority re-binding | Jason Lin | Proposed — appointment pending | Existing M001 Product / Service Owner record | Yes |
| SQ-AUTH-002 | Mission Coordination Authority re-binding | Robin Koh | Proposed — appointment pending | Existing M001 Mission Owner record | Yes |
| SQ-AUTH-003 | Engineering Authority | Ka Chen | Proposed — appointment pending | Leadership-approved proposal under CP-07B | Yes |
| SQ-AUTH-004 | QA Responsibility | Erica | Proposed — appointment pending | Leadership-approved proposal under CP-07B | Yes |
| SQ-AUTH-005 | Operations Responsibility | Eric | Proposed — appointment pending | Leadership-approved proposal under CP-07B | Yes |
| SQ-AUTH-006 | Product Commitment Approver | Jason Lin | Proposed — appointment pending | Leadership-approved proposal under CP-07B | Yes |
| SQ-AUTH-007 | Engineering Start Approver | Jason Lin | Proposed — appointment pending | Leadership-approved proposal under CP-07B | Yes |
| SQ-AUTH-008 | Mission Closure Authority | Jason Lin | Proposed — appointment pending | Leadership-approved proposal under CP-07B | Yes |

## Missing Authorities and candidate-identification requirements

| Authority | Candidate | Nomination basis required | Competence basis required | Independence requirement | Blocking stage |
|---|---|---|---|---|---|
| Business Acceptance Authority | Missing | Actual responsibility for or sustained use of quotation process | First-hand quotation workflow and acceptance knowledge | Independent from Mission coordination and implementation | Before M1 |
| Architecture Authority | Missing | Leadership nomination for SmartQuote architecture scope | SoR, tenant, identity, API, snapshot, repository and environment judgment | Must independently review implementation it governs | Before M1 / Gate 2 |
| Finance / Pricing Authority | Missing | Finance / Pricing leadership nomination | Channel Cost, pricing, margin, approvals, FX/rounding/tax governance | Material Pricing and Channel Cost require four-eyes | Before M1 / Gate 2 |
| Risk Review Responsibility | Missing | Risk leadership nomination | Independent risk classification and exception review | Requester cannot be sole Risk Acceptor | Route before M1; substantive before Gate 2 |
| Compliance Review Responsibility | Missing | Compliance leadership nomination | Regulatory, prohibited-activity, retention and exception judgment | Product/Engineering cannot approve own exception | Route before M1; substantive before Gate 2 |
| Security Review Responsibility | Missing | Security leadership nomination | Identity, permission, tenant isolation, encryption, secrets and audit judgment | Admin/developer cannot approve own access/control | Before Gate 2 / staging |
| Release Authority | Missing | Leadership / Operations governance nomination | Release evidence, rollback and operational judgment | Separate from author/deployer for material release | Before staging / production |
| Sales Representative | Missing | Sales leadership nomination | Current quotation process and internal-user facts | Cannot approve own Pricing exception | Before M1 |
| Channel Cost Accountable Contact | Missing | Finance / Channel leadership nomination | Current owner, SoR and maintenance-process knowledge | Cannot self-approve material cost changes | Before Gate 2 |

## Conflict and independence controls

### Jason Lin concentration

Jason is proposed for Product Authority, Product Commitment Approver, Engineering Start Approver and Mission Closure Authority. These remain separate decisions.

Controls:

- each Authority requires explicit acceptance;
- Commitment and Engineering Start rely on independent Architecture, Engineering, QA, Operations and professional evidence;
- Jason must not be the sole author, reviewer and approver of the same readiness evidence;
- Production Release remains separately appointed;
- each decision requires its own record and effective date.

### Robin Koh independence

Robin coordinates M1, evidence, participants and blockers. Robin must not also act as independent Business Acceptance Authority for the same Mission.

### Ka Chen engineering independence

Ka Chen must not be the sole reviewer of code he authors or directs and must not serve as Release Approver for his own change.

### Eric operational independence

Eric must not approve his own access elevation, Security Control, production deployment or Production Release.

### Finance / Channel Cost

The maintainer, author or requester of a material Channel Cost or Pricing change must not be the sole reviewer and approver.

### Sales exception

A Sales user must not approve their own Pricing or financial exception.

### Release independence

Release Authority must review independent QA, Security and Operations evidence and remain appropriately separate from implementation and deployment execution.

## M1 professional preparation

### Required concentrated response bundle

The following should be collected in one bounded cycle rather than repeated requests:

1. Robin Product Understanding Alignment and Mission-boundary acceptance;
2. actual quotation-process facts;
3. Business Acceptance criteria;
4. actual Sales representative;
5. Finance / Pricing Authority candidate and acceptance;
6. Channel Cost owner and Source of Record;
7. Architecture Authority candidate and acceptance;
8. Risk and Compliance routes;
9. Security route;
10. Ka Chen, Erica and Eric acceptance and participation scope.

### Data boundary

Only sanitized summaries and pure synthetic examples may be supplied to AI. Real Merchant, Customer, Channel Cost, Pricing, Contract, Payment, KYC, Production or Credential data remain prohibited.

## Current readiness

### M1

`Hold / Not Passed`

Blocking items:

- Robin explicit response missing;
- Business Acceptance Authority missing;
- actual Sales representative missing;
- Architecture Authority missing;
- Finance / Pricing Authority and Channel Cost ownership missing;
- Risk / Compliance / Security routes missing;
- Engineering, QA and Operations acceptance missing;
- current quotation-process facts and baselines missing.

### Gate 2

`Hold / Not Passed`

Additional blockers include Merchant Identity SoR, tenant/identity/permission design, API boundary, snapshot integrity, repository, environment, CI/test ownership, rollback, monitoring and Shared Foundation compliance.

### Product Commitment

`Not Granted`

### Engineering Start

`Not Authorized`

No product-code repository creation, coding, real-data use, staging or production is authorized.

## Source hierarchy

1. STAR Global Decision Log and Company Minimum Control Baseline;
2. Company Authority Register;
3. this M001 Authority Record;
4. Explicit Acceptance Records;
5. applicable professional Sources of Record;
6. technical permissions and execution assignments, which do not create Authority.
