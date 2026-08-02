# STAR Company Governance Authority Model

| Field | Value |
|---|---|
| Status | Candidate |
| Leadership decision | Confirmed adoption for design use |
| Company minimum control baseline | Candidate Operational Baseline approved through Batch A |
| Policy effective status | Not Effective |
| Named appointments | None |
| Authority-holder appointments | None |
| Source | DSP-001-047, DSP-001-048 and GDEC-0020 |
| Last reviewed | 2026-08-02 |

## Purpose

Define how STAR distinguishes decision Authority from organizational role, technical permission, execution and review. This Candidate model supports Product, Architecture, Engineering, Risk, Compliance, Release and AI Governance design. Batch A establishes the minimum operational control baseline used before formal appointment, Product Commitment, Gate passage, Engineering Start, sensitive-data use or production activity.

## Core principles

1. Authority belongs only to a governed human or governing body; AI tools cannot hold company decision Authority.
2. Accountability cannot be delegated away, even when execution is delegated.
3. System permission does not create Authority.
4. Missing Authority stops the decision and cannot be inferred by AI.
5. Temporary Authority requires exact scope, evidence, effective date, expiry and revocation.
6. Professional truth remains in the professional Source of Record.
7. High-risk decisions require appropriate independence and four-eyes.
8. Unregistered or unaccepted Authority must not be presumed to exist.
9. Authority revocation and technical-access revocation are separate governed actions.

## Authority hierarchy

```text
Founder / CEO Authority
→ Executive Leadership Authority
→ Portfolio and Corporate Governance Authority
→ Product / Architecture / Engineering / Risk / Compliance / Finance / Security Authority
→ Mission / Operations / QA / Release / Incident / Records Authority
→ Execution Assignments and Technical Permissions
```

The hierarchy does not remove professional hard-block or independent-review duties.

## Confirmed role boundaries

- Product Authority owns product intent, scope and business outcome.
- Mission Authority owns coordination, dependencies, evidence and readiness.
- Mission Authority cannot alone change Product Intent, pass a Gate or authorize Delivery.
- Architecture Authority does not automatically hold Engineering or Release Authority.
- Engineering Authority does not automatically hold Product, Commercial, Risk or Compliance Authority.
- Reviewer is not automatically Approver.
- Executor is not Accountable Owner.
- Technical administrator is not automatically the approver of their own access or change.
- An organizational title, work assignment, repository permission or system permission does not by itself create company Authority.

## Minimum Authority Register

The approved Batch A operational baseline requires at least:

```text
Authority ID
Authority class
Purpose
Decision scope
Approval scope
Review scope
Execution boundary
Accountable office
Named holder
Acceptance status
Independence requirements
Required access
Source of Record
Effective date
Expiry or review trigger
Replacement authority
Revocation authority
Evidence
Status
```

Minimum statuses are Candidate, Proposed, Accepted, Effective, Suspended, Revoked, Expired and Missing.

## Authority acceptance mechanism

A continuing Authority becomes valid only after all conditions are satisfied:

1. leadership formally designates the Authority;
2. the designated person explicitly accepts;
3. scope and accountability are recorded;
4. conflicts and independence are checked;
5. the Source of Record is established;
6. effective date is recorded;
7. expiry or review trigger is recorded;
8. required access is verified separately;
9. replacement and revocation mechanisms are established.

Holding an organizational title, repository permission, system permission, Mission role or execution assignment does not satisfy these conditions.

## Mandatory four-eyes baseline

Four-eyes is mandatory for:

- Material Pricing Rule;
- Channel Cost;
- Financial Exception;
- Compliance Exception;
- Production Release;
- Security Control;
- Access Elevation;
- Confidential or Restricted AI Use;
- Production Data Access;
- Policy Activation.

Additional minimum segregation rules:

- the submitter must not be the sole approver;
- an access administrator must not approve their own elevation;
- a developer must not be the sole reviewer and Release Approver for their own high-risk production change;
- an exception requester must not be the sole Risk Acceptor.

## Risk Acceptance and Exception

The approved minimum path is:

```text
Risk Identified
→ Classified
→ Professional Review
→ Compensating Controls
→ Risk Acceptance Decision
→ Monitoring
→ Revalidation
→ Closure or Revocation
```

Temporary assumptions and Founder-led Fast Track cannot bypass:

- law or regulatory prohibition;
- customer or merchant data confidentiality;
- credential and secret protection;
- core Tenant Isolation;
- KYC or AML obligations;
- explicit customer contract restrictions;
- Production Release Authority;
- unresolved Critical Security Risk.

Monetary, commercial-exception and risk-acceptance thresholds remain Missing.

## Emergency Authority

Emergency Authority is limited to temporary containment. Every use requires:

- exact scope;
- reason;
- start time;
- notification recipients;
- expiry;
- evidence;
- retrospective review;
- restoration, closure or revocation decision.

Emergency Authority must not permanently change Policy, Product Intent or Risk disposition, must not automatically restore production and must not become continuing Authority automatically. Emergency Authority duration remains Missing.

## Founder-led Fast Track exit boundary

Founder-led Fast Track ends before:

- Policy Activation;
- Formal Appointment;
- Product Commitment;
- Gate Passage;
- Engineering Start;
- real sensitive-data use;
- production environment creation or use;
- external customer use;
- material financial decision;
- legal or compliance professional judgment.

The Batch A Fast Track Exit Checklist must be completed before any listed event. Failure to complete the checklist means the action remains Not Authorized.

## Current workstream effects

### PORT-001

- Authority design and bounded repository recording may continue.
- Draft PR #2 remains Open / Draft / Unmerged.
- Independent Review remains Leadership-deferred / Not Passed.
- Freeze and Merge remain unauthorized.

### PORT-002

- AI Governance Authority cannot replace Product, Risk, Compliance, Security or Release Authority.
- Confidential or Restricted AI use and Policy Activation require four-eyes.
- Batch A does not change SAIG Policy effectiveness, Controlled Validation, Package A, Wave A or PILOT-001 status.

### PORT-003

- Product and Mission Authority boundaries apply.
- M1, Gate 2, Product Commitment and Engineering Start remain separate decisions.
- SmartQuote may proceed only to named-Authority binding and readiness preparation until separately authorized.

### GateHub

- GateHub may proceed only to named-Authority binding, asset containment, evidence recovery and readiness preparation within its current authorized boundary.
- Batch A does not pass Gate 3, complete formal takeover or authorize Engineering Start.

## Limitations

This Candidate model and Candidate Operational Baseline do not:

- appoint any person;
- activate any policy;
- grant system, repository, environment or data access;
- pass any Gate;
- authorize Product Commitment, Engineering Start, Delivery, Release or production use;
- create monetary, pricing, risk, temporary-delegation or emergency-duration thresholds;
- replace Legal, Compliance, Finance, Security or Engineering professional judgment.

## Supersession

Any change requires a new global Decision Record identifying the changed provision, scope, effective use, non-effects and transition treatment.