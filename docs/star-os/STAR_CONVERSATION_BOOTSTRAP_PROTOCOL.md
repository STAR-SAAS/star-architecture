# STAR Conversation Bootstrap Protocol

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Confirmed working baseline; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | New domain, failed context transfer, rule conflict or change in conversation tooling |
| **Scope** | Every new, resumed or transferred STAR conversation |

## Purpose

Ensure that a new conversation inherits confirmed rules and current work without asking the user to repeat established instructions.

## Important limitation

A Markdown file does not automatically load itself into every AI conversation. Reliable inheritance requires at least one bootstrap pointer in the conversation, Project Instructions, agent instructions or an approved automation.

Recommended pointer:

> Before working, load `STARSAAS/star-architecture/docs/star-os/README.md`, then load the relevant domain Decision Log, Open Questions and Work Status. Follow the STAR Conversation Bootstrap Protocol.

## Bootstrap sequence

### 1. Identify the work boundary

State the current:

- STAR domain or workstream;
- product, program, Mission or project, if applicable;
- requested outcome;
- authoritative repositories or systems.

### 2. Load global governance

Read, in order:

1. `docs/star-os/STAR_OS_GLOBAL_WORKING_RULES.md`;
2. `docs/star-os/STAR_GLOBAL_DECISION_LOG.md`;
3. `docs/star-os/STAR_DECISION_SCOPE_AND_PROPAGATION.md`.

### 3. Load the relevant domain context

Read the domain's minimum set:

- README / Charter;
- Decision Log;
- Open Questions / Assumptions;
- Work Status or current handoff;
- active Mission or project brief;
- policies that govern the task.

Do not load unrelated domains merely because they exist.

### 4. Separate state correctly

Classify information as:

- **Confirmed** — accepted working constraint;
- **Candidate** — plausible but unproven;
- **Frozen** — formally approved stable baseline;
- **Superseded** — replaced but retained;
- **Missing** — required fact not available.

Never convert a Candidate or example into a fact during handoff.

### 5. Check conflicts and freshness

Before continuing:

- identify conflicting Decision IDs;
- check last-reviewed dates and review triggers;
- verify live GitHub, tool or operational state before claiming it;
- identify missing owners, dates, permissions or evidence.

### 6. Resume with a concise start message

The first operational update should state:

- context loaded;
- current objective;
- planned tasks;
- known blockers;
- whether user action is required.

It should not repeat the full historical narrative.

### 7. Execute, review and record

For each material task:

1. execute within confirmed scope;
2. run the Global Working Rules Self-Review Gate;
3. fix issues before continuing;
4. update durable Markdown and status records;
5. report progress concisely.

## Conversation close or transfer

Before moving work to another conversation, create or update a handoff containing:

- objective and scope;
- completed work;
- current state and next action;
- confirmed decisions and open questions;
- blockers and missing facts;
- authoritative links;
- user decisions required;
- files or records updated.

Use `STAR_CONVERSATION_HANDOFF_TEMPLATE.md`.

## Ownership

The AI or human initiating the new conversation owns the bootstrap check. The user should not be required to rediscover and restate already governed rules.
