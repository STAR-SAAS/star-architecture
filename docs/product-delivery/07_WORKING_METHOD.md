# STAR Working Method

| Field | Value |
|---|---|
| **Type / scope** | Working method — Product Delivery research, decision, design and validation |
| **Version / status** | v0.1.2 — Confirmed working method; details not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | Product Delivery maintainers |
| **Last reviewed** | 2026-07-12 |
| **Review trigger** | New confirmed work-discipline decision, recurring execution friction, real-Mission finding or freeze proposal |
| **Authoritative working source** | This repository path in Draft PR #1; `main` only after approved merge |
| **Affects** | All Product Delivery work batches, maintainers, AI contributors and future Mission teams |
| **Supersession** | None |
| **Access** | Public |

## End-to-end sequence

1. **Understand** — define the problem, value receiver, urgency and desired outcome.
2. **Map stakeholders** — identify users, workers, owners, approvers, operators, external parties, AI and systems.
3. **Research** — review primary sources, mature practice and relevant evidence.
4. **Challenge** — search for simpler alternatives, missing roles, contradictions, failure modes and unnecessary complexity.
5. **Recommend** — present a concise current-best judgment, alternatives and uncertainty.
6. **Decide** — escalate only strategic, broad or genuinely ambiguous choices.
7. **Record** — update Markdown decisions, assumptions, open questions, research and changelog.
8. **Architect and design** — create the minimum structure needed to support value and work.
9. **Implement in small changes** — automate checks and obtain human review appropriate to risk.
10. **Validate and learn** — assess customer/user outcome, operational behavior and lessons; feed them into the next decision.

## Work-batch communication

Before starting a multi-step batch:

1. list the planned tasks in execution order;
2. state whether any user or GitHub action is required;
3. continue without asking for confirmation when the work is reversible and within confirmed scope.

While the batch is underway, give concise progress updates that include:

- current task and purpose;
- completed / in-progress status;
- next action;
- blocker, if any;
- whether a user decision is needed.

Record durable status in `17_WORK_STATUS.md`; chat updates remain concise and operational.

## Required quality checks

### Readability

- One-page explanation first.
- Use short definitions and concrete examples.
- Put theory and source detail in appendices/reference layers.
- Do not make every role read the same document.

### Role and stakeholder review

At minimum, test implications for:

- customer and end user;
- product manager and project manager;
- architect and tech lead;
- frontend and backend;
- QA;
- AI team/agents;
- DevOps/SRE/operations;
- support, security, legal/compliance and other affected parties.

### Historical consistency

Before accepting a new proposal:

1. read `01_DECISION_LOG.md`;
2. check `04_SUPERSEDED_IDEAS.md`;
3. identify conflicts by ID;
4. create an explicit superseding decision when necessary;
5. update `CHANGELOG.md`.

## Working usability targets — not yet frozen

These are validation targets, not confirmed service levels:

- **30 seconds:** a user can identify the purpose of a view and the next action.
- **30 minutes:** a team member can understand the Mission context relevant to their role.
- **1 hour:** an experienced contributor can begin a well-scoped task.
- **5 working days:** a new engineer can make a useful, reviewed contribution with support.

These thresholds must be tested with real team members before becoming standards.

## Decision gate

Ask leadership only when:

- the choice materially changes STAR strategy or scope;
- the decision commits the organization to broad, costly architecture;
- there are two or more valid alternatives that require business preference;
- risk, compliance or customer impact requires accountable executive approval.

Routine research, drafting, source checks, consistency checks and reversible structure improvements should continue without repeated confirmation.
