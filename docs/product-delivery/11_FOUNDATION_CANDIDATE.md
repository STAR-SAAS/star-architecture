# STAR Product Delivery Foundation — Candidate

**Version:** v0.2.0  
**Status:** Candidate; not frozen  
**Purpose:** Explain the minimum Product Delivery model in one page before exposing deeper research or architecture.

## The problem

STAR needs to turn customer and user needs into reliable product outcomes across product, project, architecture, engineering, QA, AI, operations and governance teams. The model must preserve traceability without requiring every participant to learn the full STAR theory.

## The minimum delivery loop

```text
Value Need
    ↓
Mission
    ↓
Cross-functional Work
    ↓
Release and Operation
    ↓
Evidence and Learning
```

Five elements apply across the full loop:

1. **Ownership** — one accountable Mission Owner plus enduring product/service ownership.
2. **Decision** — consequential choices, rationale and impact are recorded.
3. **Risk and approval** — controls are proportional to customer, operational, security, compliance and financial impact.
4. **Traceability** — value, work, decisions, implementation, tests, release and feedback remain linked.
5. **Current state** — humans and AI can identify the active version, status, environment and next action.

## Minimum information objects

| Object | Simple meaning |
|---|---|
| **Value Need** | Who has what problem, why it matters and what measurable outcome is desired. |
| **Mission** | A bounded, owned, cross-functional commitment to deliver and verify a meaningful outcome. |
| **Work Item** | A concrete contribution assigned to a human, team, AI agent or system. |
| **Decision** | A consequential choice with context, rationale, owner and impact. |
| **Release** | A defined change made available to an environment or user group. |
| **Evidence** | Tests, operational results, customer feedback and metrics used to judge the outcome. |

Artifacts such as PRDs, diagrams, API specifications, code and test reports are linked representations or outputs. They are not separate top-level layers in the minimum model.

## Product structure and delivery structure are different

```text
Enduring structure: Product → Capability
Temporary delivery: Value Need → Mission → Work Item → Release → Evidence
```

A Mission may change one or more product capabilities. A Product or Capability does not end when a Mission closes.

## Mission definition

A Mission is:

> A bounded, owned, cross-functional commitment to deliver and verify a meaningful outcome for an identified value receiver.

A Mission candidate must identify:

- value receiver, problem and expected outcome;
- scope and explicit exclusions;
- accountable Mission Owner;
- contributors, approvers and affected parties;
- acceptance and evidence required for closure;
- release or operational path;
- material risks, dependencies and decisions.

A Mission is **not**:

- an enduring product such as GateHub;
- a capability such as Payment Routing;
- an individual task such as adding one database column;
- an artifact such as a PRD or architecture diagram;
- a vague aspiration such as “improve customer experience”;
- routine recurring operations with no bounded change outcome.

An incident is not automatically a Mission. A bounded recovery or prevention initiative may become one.

## Entry and exit boundaries

A Mission becomes **Committed** only when the value, owner, scope, acceptance evidence and major dependencies are clear enough to begin coordinated work.

A Mission can close only when:

- the intended change is released or otherwise operationally delivered;
- required quality, risk and approval evidence exists;
- outcome evidence has been reviewed, or a named owner and date exist for delayed measurement;
- remaining work is explicitly transferred to a Product Owner, Service Owner, backlog or follow-up Mission;
- decisions and reusable learning have been recorded.

## What every role sees first

The first Mission view should show only:

1. **Why** — problem, value receiver and expected outcome.
2. **What** — scope, exclusions and acceptance.
3. **Who** — owner, contributors, approvers and affected parties.
4. **Now** — status, next action, blockers, risks and decisions needed.
5. **Evidence** — tests, release, operational results, metrics and feedback.

Detailed research, architecture and implementation artifacts are available through drill-down links.

## Validation status

This candidate is consistent with the current Decision Log and has been desk-tested against a SmartQuote discount-rule change and a GateHub PSP connector. It still requires validation on a real active Mission with actual owners, dates, dependencies and acceptance evidence before it can be frozen.