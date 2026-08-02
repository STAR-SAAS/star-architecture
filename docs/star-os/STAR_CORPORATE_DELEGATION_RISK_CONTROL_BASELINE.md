# STAR Corporate Delegation, Risk and Control Baseline

| Field | Value |
|---|---|
| Status | Candidate Operational Baseline |
| Leadership approval | Batch A approved on 2026-08-02 |
| Policy effective status | Not Effective |
| Named appointments | None |
| Source | DSP-001-048 and Company Minimum Control Baseline Batch A |
| Last reviewed | 2026-08-02 |

## Purpose

Establish the minimum company control baseline required before formal appointment, Product Commitment, Gate passage, Engineering Start, sensitive-data use or production activity. This is a Candidate Operational Baseline: it is approved for governed operational use as a decision and readiness constraint, but it is not an effective company policy and creates no named appointment, threshold, Gate passage, Delivery or production authorization.

## A1. Company Authority Register

STAR must maintain a governed Authority Register. Role, Responsibility, Permission, Authority, Review, Approval, Execution and Accountability must be recorded separately and must not be inferred from one another.

### Minimum Authority Register fields

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

### Minimum Authority classes

```text
Product Authority
Mission Coordination Authority
Architecture Authority
Engineering Authority
Security Review Responsibility
Compliance Review Responsibility
Finance / Pricing Authority
Risk Acceptance Authority
QA / Acceptance Responsibility
Operations Authority
Release Authority
Incident / Emergency Authority
Records Authority
Policy Activation Authority
```

### Authority status

```text
Candidate
Proposed
Accepted
Effective
Suspended
Revoked
Expired
Missing
```

`Named holder` and `Acceptance status` remain empty until a separately authorized appointment and explicit acceptance occur. Unregistered or unaccepted Authority must not be presumed to exist.

## A2. Appointment, Acceptance, Revocation and Replacement

A continuing Authority becomes valid only after all required conditions are satisfied:

1. leadership formally designates the Authority;
2. the designated person explicitly accepts;
3. exact scope and accountability are recorded;
4. conflict and independence checks are completed;
5. the Source of Record is established;
6. effective date is recorded;
7. expiry or review trigger is recorded;
8. required access is verified separately;
9. replacement and revocation mechanisms are established.

The following do not automatically create company Authority:

- organizational title;
- job responsibility;
- GitHub permission;
- system or environment permission;
- Mission ownership;
- task assignment;
- prior execution of similar work;
- attendance, silence or lack of objection.

Authority revocation and system-access revocation are separate actions. Revoking Authority does not by itself remove technical access, and removing technical access does not by itself revoke recorded Authority.

### Delegation fields

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

Temporary delegation duration remains Missing and must not be invented or inferred.

## A3. Four-eyes and Segregation of Duties

Critical or material decisions must not rely on self-approval.

Minimum rules:

- the submitter must not be the only approver;
- an access administrator must not approve their own access elevation;
- a developer must not be the sole reviewer and Release Approver for their own high-risk production change;
- an exception requester must not be the sole Risk Acceptor;
- a reviewer is not automatically an approver;
- an executor is not automatically accountable for the decision;
- system administration permission does not create approval Authority.

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

## A4. Risk Acceptance and Exception

### Required process

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

### Minimum Risk / Exception Register fields

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

### Non-bypassable boundaries

The following cannot be bypassed through ordinary exception, temporary assumption, system permission or Founder-led Fast Track:

1. law or regulatory prohibition;
2. customer or merchant data confidentiality;
3. credential and secret protection;
4. core Tenant Isolation;
5. KYC / AML obligations;
6. customer contract restrictions;
7. Production Release Authority;
8. unresolved Critical Security Risk.

The following thresholds remain Missing:

- monetary thresholds;
- commercial exception thresholds;
- risk acceptance thresholds.

Missing thresholds do not authorize action. They require escalation when a decision depends on them.

## A5. Emergency Authority

Emergency Authority is limited to temporary containment.

Every emergency action must record:

```text
Action ID
Actor
Authority basis
Exact scope
Reason
Start time
Affected systems
Notification recipients
Expiry
Evidence
Retrospective review
Restoration decision
Closure or revocation
```

Emergency Authority may support actions such as stopping an affected system, pausing deployment, revoking dangerous access, isolating an environment or containing an incident.

Emergency Authority must not:

- permanently change policy;
- permanently change Product Intent;
- permanently accept or alter risk disposition;
- automatically restore production;
- automatically become continuing Authority.

Emergency Authority duration remains Missing and must not be invented or inferred.

## A6. Founder-led Fast Track Exit Checklist

Founder-led Fast Track must end before any of the following:

1. Policy Activation;
2. Formal Appointment;
3. Product Commitment;
4. Gate Passage;
5. Engineering Start;
6. real sensitive-data use;
7. production environment creation or use;
8. external customer use;
9. material financial decision;
10. legal or compliance professional judgment.

Before any listed event, the responsible workstream must complete a Fast Track Exit Checklist confirming:

```text
Decision or action requested
Applicable Authority
Named holder
Acceptance evidence
Required professional reviews
Four-eyes requirement
Data classification
Environment classification
Non-bypassable boundary check
Risk / exception status
Source of Record
Effective date
Expiry or review trigger
Leadership decision
```

Failure to complete the checklist means the action remains Not Authorized.

## Product binding preparation

### SmartQuote

Prepare binding for Product Authority, Mission Coordination Authority, Architecture Authority, Engineering Authority, Business Acceptance, Finance / Pricing, Risk, Compliance, QA, Engineering Start and Release Authority before the applicable M1, Gate 2, Product Commitment, Engineering Start, staging or production decision.

### GateHub

Prepare binding for Product / Service Authority, Handover Acceptance, Repository Ownership, Architecture, Engineering, Data, Security, Compliance, QA, Operations, Engineering Start, Release and Incident Authority before formal takeover, Engineering Start, staging or production deployment.

### STAR AI Governance

Prepare binding for AI tool approval, AI data use, Confidential or Restricted AI use, AI-generated work review, policy activation and continuity. SAIG Authority does not replace Product, Risk, Compliance, Security or Release Authority.

## Thresholds remaining Missing

The following are intentionally not set by Batch A:

- monetary thresholds;
- commercial exception thresholds;
- risk acceptance thresholds;
- temporary delegation duration;
- Emergency Authority duration;
- committee composition;
- named Authority holders.

## Non-effects

This Candidate Operational Baseline does not:

- appoint any person or committee;
- activate any policy;
- approve monetary, commercial, risk or duration thresholds;
- grant system, repository, environment or data access;
- convert technical permission into company Authority;
- pass M1, Gate 2, Gate 3 or any other Gate;
- authorize SmartQuote Engineering Start;
- authorize GateHub Engineering Start;
- authorize Product Commitment, Delivery, Release or production use;
- change Draft PR #2 Ready, Freeze or Merge status;
- replace Legal, Compliance, Finance, Security or Engineering professional judgment.