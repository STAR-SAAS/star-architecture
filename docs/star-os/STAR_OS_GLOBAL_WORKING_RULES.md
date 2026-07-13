# STAR OS Global Working Rules

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Confirmed working baseline; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | Global-rule change, repeated execution failure, cross-domain conflict or freeze proposal |
| **Authoritative working source** | This repository path in its Draft PR; `main` only after approved merge |
| **Scope** | All STAR conversations, domains, products, Missions, projects and human/AI contributors |
| **Access** | Public; sensitive operational records belong in approved private systems |

## Purpose

These rules prevent confirmed working disciplines from being lost when work moves between conversations, teams, projects or AI tools.

## The rules

### GWR-01 — Understand before building

Define the problem, value receiver, desired outcome, constraints and missing facts before proposing architecture or implementation.

### GWR-02 — Research and evidence before invention

Use credible evidence and mature practices before creating a STAR-specific replacement. Distinguish fact, industry practice, assumption and proposal.

### GWR-03 — Plan multi-step work before execution

Before a material batch:

1. list the tasks in execution order;
2. state whether user or GitHub action is required;
3. continue without repeated approval when the work is reversible and inside confirmed scope.

### GWR-04 — Report progress while work is active

Progress updates must state:

- current task and purpose;
- completed / in-progress status;
- next action;
- blocker, if any;
- whether a user decision is required.

### GWR-05 — Review before continuing

After every material task or document, complete the Self-Review Gate before starting the next task. Fix discovered issues first.

#### Self-Review Gate

- Is the requested outcome complete?
- Is every factual claim supported or clearly marked uncertain?
- Does the result conflict with a confirmed Decision ID?
- Is it concise and understandable for the intended audience?
- Were customers, users and all affected stakeholders considered?
- Are Candidate, Confirmed, Frozen and Superseded states used correctly?
- Were Markdown records, status and links updated where required?
- Was any completion, synchronization or validation claim actually verified?

### GWR-06 — Make complexity progressive

Provide a simple first view. Put detailed architecture, research and reference material behind drill-down links. Do not require every role to read the entire theory.

### GWR-07 — Record durable memory

Chat is working context, not durable organizational memory. Every material confirmed decision must enter the appropriate versioned Markdown record with scope and provenance.

### GWR-08 — Apply rules by scope

Every material rule or decision must declare its scope. Global rules propagate to all STAR work; narrower rules propagate only to their stated domain, product, Mission, conversation or task.

### GWR-09 — Do not silently override history

A new proposal that conflicts with an active decision must identify the affected Decision ID and explicitly supersede it, request an exception or be rejected.

### GWR-10 — Escalate only accountable decisions

Ask leadership when a choice changes strategy or scope, commits broad or costly architecture, carries material customer/security/compliance/financial risk, or requires business preference between valid alternatives. Routine reversible work continues without repeated confirmation.

### GWR-11 — Proactively identify missing participants

Do not rely only on roles named by the requester. Check customers, end users, product, project, architecture, engineering, QA, AI, operations, support, security, legal/compliance, finance, partners, regulators and participating systems as relevant.

### GWR-12 — Never manufacture evidence

Missing owners, dates, approvals, system state, customer facts or validation results remain explicit gaps. Plausible examples are not evidence of real execution.

## Enforcement

- New STAR conversations load these rules through the Conversation Bootstrap Protocol.
- Domain and project rules may add detail but may not silently weaken these rules.
- An exception requires an owner, rationale, exact scope, expiry/review trigger and approval.
- Repeated failure of a rule triggers review of the rule, workflow or supporting tooling rather than repeated reminders to individual users.
