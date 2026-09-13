# STAR Delivery Model — Initial Validation

**Version:** v0.1.0  
**Date:** 2026-07-12  
**Status:** Candidate validation; not frozen

## Question being tested

Can a simple chain — **need/value → Mission → work → release → learning** — support real STAR product delivery without forcing every role to understand the full theory?

## Case A — SmartQuote: merchant-specific discount rule

### Need and value

- **Value receiver:** merchant sales/quotation user and the merchant business.
- **Problem:** negotiated discounts are handled manually or inconsistently.
- **Desired outcome:** produce accurate quotes faster, with controlled and auditable discount rules.

### Candidate Mission

> Deliver configurable merchant-specific discount rules in SmartQuote, with approval, calculation, display, testing and auditability.

### Minimum cross-functional work

| Participant | Needs to know | Produces / decides |
|---|---|---|
| Customer / end user | What changes in quotation behavior and when it is available | Feedback and acceptance evidence |
| Product manager | Business rule, affected users, scope, success measure | Requirement and priority |
| Project manager | Dependencies, milestones, owners and blockers | Delivery plan and coordination |
| Architect | Rule boundary, configuration approach, audit and integration impact | Decision record and design constraints |
| Backend | Pricing inputs, precedence, API and data impact | Rule execution and API changes |
| Frontend | Display, explanation, permissions and error states | User interaction changes |
| QA | Acceptance rules, edge cases and regression scope | Test evidence |
| AI team / agents | Authorized rules, current design and task boundary | Draft analysis/code/tests subject to review |
| Operations / support | Rollout, monitoring, failure handling and customer explanation | Operational readiness and support material |
| Compliance / finance if applicable | Discount authority and audit requirements | Approval constraints |

### Outcome measures to consider

- quote preparation time;
- pricing error rate;
- percentage of discount exceptions handled without manual intervention;
- support incidents after release;
- user acceptance/usage.

## Case B — GateHub: add a new PSP connector

### Need and value

- **Value receiver:** merchant/customer needing additional payment coverage and payment users seeking successful transactions.
- **Problem:** current provider coverage, acceptance, geography, payment methods or commercial terms are insufficient.
- **Desired outcome:** safely route eligible transactions through a new PSP with measurable operational reliability.

### Candidate Mission

> Integrate and release a production-ready PSP connector, including commercial/compliance readiness, API mapping, failure handling, reconciliation signals, monitoring and rollback.

### Minimum cross-functional work

| Participant | Needs to know | Produces / decides |
|---|---|---|
| Customer / merchant | Supported methods/markets, onboarding requirements and launch date | Pilot feedback and acceptance evidence |
| Product manager | Customer value, supported scenarios and exclusions | Scope and success criteria |
| Project manager | External dependency dates, certification, sandbox and production readiness | Integrated delivery plan |
| Architect | Connector boundary, canonical payment model, idempotency, security and failure semantics | ADR/design and integration contract |
| Backend | Authentication, request/response mapping, webhooks, retries and persistence | Connector implementation |
| Frontend / portal | Configuration, status, error and operational views if needed | UI changes only where required |
| QA | Sandbox scenarios, negative paths, contract, resilience and regression coverage | Test/certification evidence |
| AI team / agents | Provider docs, canonical model, decisions and security constraints | Draft mappings/tests/docs subject to review |
| DevOps/SRE/Ops | Secrets, deployment, alerts, dashboards, incident and rollback procedures | Operational readiness and runbook |
| Risk/compliance/legal/finance | Provider due diligence, data handling, settlement/commercial obligations | Required approvals and controls |
| Partner / PSP | API specifications, credentials, certification and incident contacts | External readiness and support commitment |

### Outcome measures to consider

- transaction acceptance and technical success rates;
- latency and timeout rate;
- webhook/reconciliation completeness;
- incident and rollback frequency;
- merchant adoption and transaction volume;
- cost or routing benefit.

## Findings

### The simple chain is useful, but incomplete by itself

Both cases can be described as:

```text
Need / Value
    ↓
Mission
    ↓
Cross-functional Work
    ↓
Release and Operation
    ↓
Measured Outcome and Learning
```

However, five cross-cutting elements are required throughout:

1. **Ownership** — Mission owner and enduring product/service owner are not always the same.
2. **Decision** — important choices and trade-offs require explicit records.
3. **Risk and approval** — controls vary by impact; one universal process would be wasteful.
4. **Traceability** — requirements, API/data, tests, release and feedback must link without forcing one giant document.
5. **Current state** — status, version and environment matter for both humans and AI.

## Candidate minimum information model

This is a deliberately small candidate, not a frozen meta-model:

| Item | Purpose |
|---|---|
| Value Need | Defines who has what problem and the desired measurable outcome. |
| Mission | Bounded cross-functional commitment to achieve an outcome. |
| Work Item | Specific contribution required from a person, team, AI agent or system. |
| Decision | Records a consequential choice, rationale and impact. |
| Release | Identifies the change delivered to an environment or user group. |
| Feedback / Evidence | Captures customer, operational and quality results after delivery. |
| Relationships | Links owners, stakeholders, artifacts, risks and dependencies to the items above. |

Artifacts such as PRDs, APIs, diagrams, code and test reports can remain linked representations rather than becoming separate top-level concepts in the first model.

## Readability test

A team-facing Mission view should initially show only:

1. **Why:** problem, value receiver and expected outcome.
2. **What:** scope, exclusions and acceptance.
3. **Who:** owner, contributors, approvers and affected parties.
4. **Now:** status, next action, blockers and decisions needed.
5. **Evidence:** release, tests, metrics and feedback.

Architecture, research and detailed artifacts should be available by drill-down, not placed on the first screen.

## Current conclusion

The candidate chain is strong enough to continue testing, but it is **not ready to freeze**. The next useful validation is to take one actual upcoming SmartQuote or GateHub change, populate these fields with real owners and acceptance criteria, and observe where the model creates friction or misses information.
