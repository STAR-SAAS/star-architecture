# STAR Corporate Delegation, Risk and Control Baseline

| Field | Value |
|---|---|
| Status | Candidate preparation record |
| Policy effective status | Not Effective |
| Named appointments | None |
| Source | DSP-001-048 |
| Last reviewed | 2026-07-21 |

## Purpose

Prepare the next governance batch without confirming thresholds, appointments or policy activation.

## Candidate design scope

1. Company Authority Register;
2. Corporate Delegation of Authority;
3. monetary, commercial and risk threshold decision package;
4. Risk Acceptance and Exception Register;
5. Four-eyes and Segregation-of-Duties Standard;
6. Emergency Authority and Incident Escalation Matrix;
7. Product / Architecture / Engineering / Release RACI;
8. Authority Acceptance mechanism;
9. temporary delegation and expiry model;
10. SmartQuote, GateHub and SAIG Authority binding plan.

## Authority Register candidate fields

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

`Named holder` and `Acceptance status` remain empty until a separately authorized appointment and explicit acceptance occur.

## Delegation candidate fields

```text
Delegation ID
Delegating Authority
Delegate
Decision class
Exact scope
Maximum value or risk level
Start date
Expiry
Evidence
Required reviewers
Non-delegable elements
Revocation authority
Status
```

## Risk Acceptance and Exception Register candidate fields

```text
Exception ID
Risk class
Risk level
Decision owner
Risk acceptor
Required reviewers
Exact scope
Reason
Compensating controls
Evidence
Start date
Expiry
Revalidation trigger
Revocation authority
Exit plan
Status
```

## Four-eyes and segregation baseline

The next batch must define submitter, reviewer, approver and executor combinations for each material decision class. It must prohibit self-approval for access elevation, material commercial exception, production release and other high-risk changes.

## Emergency and incident baseline

The next batch must distinguish:

- emergency containment;
- incident declaration;
- temporary suspension;
- recovery authorization;
- permanent change;
- retrospective review.

Emergency action must never silently establish permanent Authority.

## Authority acceptance candidate mechanism

Continuing Authority requires:

1. formal leadership designation;
2. explicit acceptance by the designated person;
3. recorded scope and accountability;
4. conflict and independence check;
5. established Source of Record;
6. effective date;
7. expiry or review trigger;
8. separately verified required access;
9. replacement and revocation mechanism.

An organizational title alone does not constitute Authority acceptance.

## Thresholds remaining Missing

The following are intentionally not set:

- financial approval thresholds;
- Material Pricing or pricing-exception thresholds;
- Channel Cost exception thresholds;
- risk acceptance thresholds;
- maximum temporary-delegation duration;
- maximum Emergency Authority duration;
- committee composition;
- named Authority holders.

These values require a separate leadership decision package and appropriate professional input.

## Product binding preparation

### SmartQuote

Prepare binding for Product Authority, Mission Authority, Architecture Authority, Engineering Authority, Business Acceptance, Finance, Commercial Rule, Risk, Compliance, QA and Release Authority before the applicable M1, Gate 2, Commitment, Delivery or Production decision.

### GateHub

Prepare binding for repository and code ownership, Architecture, Engineering, Data, Security, Compliance, Operations, Release and Incident Authority before handover, migration, formal takeover or production deployment.

### STAR AI Governance

Prepare binding for AI tool approval, AI data use, Confidential or Restricted AI use, AI-generated work review, policy activation and continuity. SAIG Authority does not replace Product, Risk, Compliance, Security or Release Authority.

## Non-effects

This preparation record does not:

- create or activate policy;
- appoint any person or committee;
- approve thresholds;
- grant access;
- pass a Gate;
- authorize Product Commitment, Engineering Start, Delivery, Release or production use;
- change SAIG, SmartQuote or GateHub professional status.