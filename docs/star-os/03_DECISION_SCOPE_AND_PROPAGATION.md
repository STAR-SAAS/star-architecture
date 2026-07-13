# STAR Decision Scope and Propagation Model

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Confirmed working model; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | Scope conflict, new organizational layer, exception failure or freeze proposal |
| **Authoritative working source** | This file in the active Draft PR; `main` only after approved merge |

## Scope levels

| Scope | Applies to | Example |
|---|---|---|
| **Global** | Every STAR workstream, conversation, product, Mission, human and AI contributor | Do not ask the user to reconfirm recorded decisions merely because the conversation changed |
| **Domain** | One long-lived area and all subordinate work | Product Delivery or AI Governance |
| **Product / Program** | One product or enduring program and its Missions | SmartQuote or GateHub |
| **Project / Mission** | One bounded initiative or delivery commitment | Mission-001 or Mission-002 |
| **Conversation / Task** | One temporary discussion or work batch | A bounded repository documentation update |

## Mandatory decision metadata

Every material decision should identify:

- Decision ID and title;
- scope;
- status: Proposed, Confirmed, Frozen, Rejected or Superseded;
- accountable owner;
- effective date and review trigger;
- authoritative source;
- applies-to / propagation targets;
- affected stakeholders and systems;
- supersedes / superseded-by relationship;
- exception or expiry condition where relevant.

## Propagation rules

1. **Global decisions propagate to all subordinate scopes.**
2. **Domain decisions propagate to products, Missions and conversations within that domain.**
3. **Product decisions propagate to that product's projects and Missions.**
4. **Mission decisions stay within the Mission unless explicitly promoted.**
5. **Conversation/task decisions expire with the task unless recorded and promoted.**
6. **Narrower rules may add detail but may not silently contradict broader rules.**
7. **Sensitive records do not propagate by copying.** Their policy and references may propagate; the data remains in its authorized source.

## Conflict handling

When two applicable records conflict:

1. check whether one explicitly supersedes the other;
2. check scope and effective date;
3. apply mandatory legal, regulatory, security and customer-safety constraints;
4. prefer the valid broader rule unless a recorded exception authorizes specialization;
5. stop material action when authority is unclear;
6. cite both Decision IDs and request only the decision needed to resolve the conflict.

A newer narrow decision cannot silently override a Global decision.

## Promotion and demotion

- **Promote** a decision when repeated use proves that it should apply to a broader scope.
- **Demote or specialize** when a broad decision is too general and a narrower rule is needed.
- **Supersede** when the old decision is no longer the current rule.
- **Archive** when the scope no longer exists but historical traceability is still useful.

Promotion, demotion and supersession require a new Decision ID and a link to the earlier record.

## Inheritance check

Before a material task starts, determine:

```text
Global rules → Domain rules → Product/Program rules → Mission rules → Task authorization
```

The final task context should contain only the applicable subset, not every rule in the organization.
