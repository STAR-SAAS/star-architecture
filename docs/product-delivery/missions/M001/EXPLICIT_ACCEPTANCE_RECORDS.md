# M001 · Explicit Acceptance Records

| Field | Value |
|---|---|
| Work item | CP-07B · SmartQuote Named Authority Appointment and Explicit Acceptance |
| Leadership authorization | Approved by Jason Lin on 2026-08-02 |
| Record status | Prepared — responses not yet received |
| Effective appointments | None created by this record |
| Last reviewed | 2026-08-02 |

## Acceptance rule

A proposed Authority remains `Proposed — appointment pending` until the proposed holder explicitly responds with `Accept` or `Accept with clarification`, all material conflicts are resolved, required conditions are recorded and the appointment is separately made effective.

Silence, meeting attendance, no objection, job title, Mission role, GitHub permission, system permission or prior execution does not constitute acceptance.

## Consolidated acceptance template

```text
Authority ID:
Authority:
Proposed holder:
Exact scope:
Responsibility:
Accountability:
Explicit exclusions:
Required independence:
Required four-eyes:
Required access:
Source of Record:
Proposed effective date:
Review trigger:
Replacement route:
Revocation route:

Response:
- Accept
- Accept with clarification
- Decline

Clarification:
Conflict disclosure:
Current access:
Access still required:
```

## Acceptance records

### SQ-AUTH-001 · Product Authority re-binding

```text
Proposed holder: Jason Lin
Status: Proposed — appointment pending
Response: Missing
Conflict disclosure: Missing
Current access: Not assessed in this record
Access still required: To be verified separately
Proposed effective date: Pending acceptance and leadership effectiveness decision
```

### SQ-AUTH-002 · Mission Coordination Authority re-binding

```text
Proposed holder: Robin Koh
Status: Proposed — appointment pending
Response: Missing
Conflict disclosure: Missing
Current access: Not assessed in this record
Access still required: To be verified separately
Proposed effective date: Pending acceptance and leadership effectiveness decision
Additional required response: Product Understanding Alignment and Mission-boundary acceptance
```

### SQ-AUTH-003 · Engineering Authority

```text
Proposed holder: Ka Chen
Status: Proposed — appointment pending
Response: Missing
Conflict disclosure: Missing
Current access: Not assessed in this record
Access still required: Company repository and approved dev/test environment after separate authorization
Proposed effective date: Pending acceptance and leadership effectiveness decision
Independence condition: Not sole reviewer or Release Approver for own work
```

### SQ-AUTH-004 · QA Responsibility

```text
Proposed holder: Erica
Status: Proposed — appointment pending
Response: Missing
Conflict disclosure: Missing
Current access: Not assessed in this record
Access still required: Requirements, test environment and CI evidence after separate authorization
Proposed effective date: Pending acceptance and leadership effectiveness decision
Independence condition: QA evidence remains independent from implementation
```

### SQ-AUTH-005 · Operations Responsibility

```text
Proposed holder: Eric
Status: Proposed — appointment pending
Response: Missing
Conflict disclosure: Missing
Current access: Not assessed in this record
Access still required: Approved dev/test environment after separate authorization
Proposed effective date: Pending acceptance and leadership effectiveness decision
Independence condition: Cannot approve own access elevation, Security Control, deployment or Release
```

### SQ-AUTH-006 · Product Commitment Approver

```text
Proposed holder: Jason Lin
Status: Proposed — appointment pending
Response: Missing
Conflict disclosure: Missing
Current access: Not applicable as decision Authority; evidence access to be verified
Access still required: M1, Gate 2, professional-risk and resource evidence
Proposed effective date: Pending acceptance and leadership effectiveness decision
Independence condition: Must rely on independent readiness evidence
```

### SQ-AUTH-007 · Engineering Start Approver

```text
Proposed holder: Jason Lin
Status: Proposed — appointment pending
Response: Missing
Conflict disclosure: Missing
Current access: Not applicable as decision Authority; evidence access to be verified
Access still required: Architecture, Engineering, QA and Operations readiness evidence
Proposed effective date: Pending acceptance and leadership effectiveness decision
Independence condition: Product Commitment does not automatically authorize Engineering Start
```

### SQ-AUTH-008 · Mission Closure Authority

```text
Proposed holder: Jason Lin
Status: Proposed — appointment pending
Response: Missing
Conflict disclosure: Missing
Current access: M0–M4 evidence access to be verified
Access still required: Business Acceptance, Mission, QA, Operations and risk evidence
Proposed effective date: Pending acceptance and leadership effectiveness decision
Independence condition: Closure cannot rely solely on Product Authority judgment
```

## Concentrated response bundle

The acceptance request should be delivered once to the relevant proposed holders, with only role-specific sections exposed to each recipient. It should also collect:

- Robin Product Understanding Alignment;
- actual quotation-process facts from an actual Sales user;
- Business Acceptance criteria;
- Finance / Pricing ownership and Channel Cost owner / SoR;
- Architecture, Risk, Compliance and Security routes;
- Engineering, QA and Operations participation scope and availability.

## Delivery status

`Prepared — not sent`

Reason: recipient email addresses or another authorized delivery channel were not available to the executing AI. No acceptance response may be inferred.

## Current gate state

```text
M1: Hold / Not Passed
Gate 2: Hold / Not Passed
Product Commitment: Not Granted
Engineering Start: Not Authorized
```
