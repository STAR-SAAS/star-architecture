# STAR Decision Scope and Propagation Model

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Confirmed working baseline; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | Cross-domain conflict, new scope level, failed propagation or exception abuse |
| **Scope** | All material STAR rules, decisions, policies and exceptions |

## Purpose

Ensure that a confirmed decision reaches every place where it applies, without copying every rule into every project or conversation.

## Scope levels

| Scope | Applies to | Example |
|---|---|---|
| **Global** | All STAR work | Review each material task before continuing |
| **Domain** | One STAR domain | AI tool approval rules in STAR AI Governance |
| **Product / Program** | One enduring product or program | GateHub payment architecture constraints |
| **Mission / Project** | One bounded delivery or project | Mission-002 release acceptance |
| **Conversation** | One working thread | Temporary discussion format |
| **Task** | One authorized action | AI may update named files on one branch |

## Required decision fields

Every material decision should record:

- **Decision ID and title**;
- **status** — Proposed, Confirmed, Frozen, Rejected or Superseded;
- **scope**;
- **applies to** — named domains, products, Missions, teams, systems or AI agents;
- **owner and approver**;
- **decision and rationale**;
- **effective date**;
- **authoritative source**;
- **propagation targets**;
- **review trigger or expiry**;
- **supersedes / superseded by**;
- **exceptions**, if any.

## Propagation rules

### Global decision

Update:

1. `STAR_GLOBAL_DECISION_LOG.md`;
2. the affected global rule or protocol;
3. relevant domain bootstrap pointers or indexes;
4. active handoffs or Work Status files where execution changes.

Do not copy the full rule into every domain. Link to the global source and record only domain-specific implementation detail.

### Domain decision

Update:

1. the domain Decision Log;
2. affected policies, templates or Work Status;
3. active product/Mission handoffs governed by the decision.

It must not be presented as a company-wide rule unless promoted through a Global decision.

### Product / Mission decision

Update the relevant Product or Mission record, affected artifacts and participant handoff. It does not automatically affect unrelated products or Missions.

### Conversation or Task decision

Record it in the current handoff or task authorization. Promote it only when evidence shows that it should become a reusable higher-scope rule.

## Conflict order

```text
Global
  ↓
Domain
  ↓
Product / Program
  ↓
Mission / Project
  ↓
Conversation
  ↓
Task
```

A lower scope may add detail but cannot silently contradict a higher active rule.

When conflict exists, choose one:

1. comply with the higher rule;
2. request an explicit exception;
3. propose a higher-level superseding decision;
4. stop the conflicting work.

## Exception record

An exception must state:

- rule or Decision ID being varied;
- exact scope;
- business reason;
- risk accepted;
- accountable owner and approver;
- start and expiry date;
- compensating controls;
- review and exit plan.

An exception is not a silent precedent. Wider adoption requires a new decision.

## Propagation check

Before closing a decision task, verify:

- the authoritative decision was updated;
- every affected active workstream can discover it;
- no unrelated scope was polluted;
- conflicting older guidance was superseded or linked;
- AI context packages reference the current source;
- the Changelog or Work Status reflects material operational impact.
