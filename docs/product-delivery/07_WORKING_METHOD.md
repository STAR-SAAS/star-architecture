# STAR Working Method

**Version:** v0.1.0  
**Status:** Confirmed working method; details not frozen

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
