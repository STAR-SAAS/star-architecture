# STAR Product Delivery Validation Plan

**Version:** v0.1.0  
**Status:** Candidate execution plan; not frozen  
**Purpose:** Turn the current Product Delivery model from a plausible design into evidence from real work.

## What must be proven

Before the foundation can be frozen, STAR must show that it:

1. helps every participant understand the Mission and their next action;
2. keeps customer/user value visible from request through operation;
3. supports product, project, architecture, engineering, QA, AI, operations and governance without one giant document;
4. preserves ownership, decisions, risk, traceability and current state;
5. avoids duplicating live information across GitHub and operational tools;
6. works on real delivery, not only desk examples.

## Validation sequence

### V1 — Real Mission walkthrough

Use `templates/MISSION_BRIEF.md` for one active SmartQuote or GateHub change.

**Participants:** customer-facing representative, product manager, project/delivery manager, architect/tech lead, frontend/backend as relevant, QA, AI representative, operations/support and affected governance roles.

**Pass evidence:**

- value receiver, problem and measurable outcome are clear;
- one Mission Owner and enduring Product/Service Owner are named;
- scope, exclusions, risks, dependencies and approvals are visible;
- every participant can state their next action and required evidence;
- detailed information is linked rather than copied;
- missing or unnecessary fields are recorded.

### V2 — Mission lifecycle observation

Follow the same Mission through commitment, implementation, release/operation and outcome review.

**Pass evidence:**

- state changes reflect reality rather than reporting convenience;
- code completion is not treated as Mission completion;
- release, quality, operational and customer evidence are linked;
- remaining ownership is explicit at closure;
- learning produces a decision, backlog item, standard update or justified no-action outcome.

### V3 — Decision-record test

Apply `templates/DECISION_RECORD.md` to:

1. one product decision;
2. one architecture/engineering decision;
3. one risk, operational or governance decision.

**Pass evidence:** one generic format remains understandable across all three. Create specialized record types only when a real gap is demonstrated.

### V4 — Role-view comprehension test

Ask representative participants to open the Mission Brief without reading the research repository first.

**Questions:**

- What is this Mission trying to achieve?
- What is your responsibility?
- What is the next action?
- What is blocked or awaiting decision?
- What evidence proves completion?

**Pass evidence:** answers are correct, fast and do not require the full theory. Record confusion by role instead of blaming the participant.

### V5 — AI work-control test

Test `14_AI_WORK_GOVERNANCE.md` on:

- one analysis/document task;
- one code or test proposal;
- one reversible tool execution in a branch or sandbox;
- one high-impact scenario as a dry run only.

**Pass evidence:** task scope, authorized context, allowed actions, reviewer, logs, stop conditions and outcome evidence are clear. AI does not silently acquire approval authority.

### V6 — Authoritative-source map

Map STAR's actual issue tracking, CRM, support, observability, CI/CD, IAM, finance and legal/compliance systems against `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md`.

**Pass evidence:** every material information class has one owner and authoritative source; GitHub links to live systems instead of duplicating their mutable state.

## Evidence register

| Validation | Status | Owner | Evidence link | Findings / next action |
|---|---|---|---|---|
| V1 Real Mission walkthrough | Not started |  |  |  |
| V2 Mission lifecycle observation | Not started |  |  |  |
| V3 Decision-record test | Not started |  |  |  |
| V4 Role-view comprehension | Not started |  |  |  |
| V5 AI work-control test | Not started |  |  |  |
| V6 Authoritative-source map | Not started |  |  |  |

## Freeze gate

The foundation may be proposed for freeze only when:

- at least one real Mission completes V1 and V2;
- no critical stakeholder or ownership gap remains;
- role-view testing shows that teams can act without reading the research history;
- AI boundaries have been tested at the relevant work levels;
- information ownership and source boundaries are explicit;
- unresolved limitations are documented and accepted rather than hidden;
- any new confirmed conclusions are recorded in the Decision Log.

A successful desk review is not enough to pass this gate.