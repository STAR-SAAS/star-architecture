# STAR Conversation Handoff Template

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Confirmed working template; not frozen |
| **Scope** | Any STAR workstream split, transfer or new conversation |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | Failed handoff, missing context, new workstream type or freeze proposal |
| **Authoritative working source** | This file in the active Draft PR; `main` only after approved merge |

## Purpose

Transfer the minimum durable context needed to continue work without asking the user to repeat previously confirmed decisions.

A handoff is a navigation record. It links authoritative sources; it does not replace Decision Logs, Charters, Work Status or project repositories.

## Handoff record

```md
# [Workstream] Conversation Handoff

## Identity
- Conversation / workstream:
- Parent scope:
- Domain / product / Mission:
- Accountable owner:
- Maintainer:
- Access classification:
- Last updated:

## Authoritative sources
- Global governance:
- Domain Charter / Decision Log:
- Product / Mission records:
- Current Work Status:
- Other authoritative systems:

## Inherited decisions
- Applicable Global Decision IDs:
- Applicable Domain Decision IDs:
- Applicable Product / Mission Decision IDs:
- Recorded exceptions:
- Superseded decisions that must not be reused:

## Current state
- Purpose:
- Current objective:
- Completed:
- In progress:
- Current blockers:
- Open questions:
- Current assumptions:
- Next evidence-producing task:
- User decision required now: Yes / No

## Sensitive-data boundary
- Information allowed in this conversation:
- Information that must remain in a private or specialized system:

## Destination startup instruction
Run `02_CONVERSATION_BOOTSTRAP_PROTOCOL.md`, read the sources above, and continue within the inherited scope. Do not ask the user to reconfirm existing decisions unless a documented change, exception or conflict requires it.
```

## Handoff rules

1. Update the source workstream's durable records before creating the handoff.
2. Link authoritative records instead of copying large amounts of content.
3. Mark candidates, assumptions and confirmed decisions separately.
4. Name blockers and missing facts; do not invent them.
5. Record sensitive-data restrictions explicitly.
6. Register the destination workstream in `04_WORKSTREAM_REGISTRY.md`.
7. The destination conversation must run the Bootstrap Protocol before material work.
8. A handoff expires when its linked Work Status or decisions materially change; update it rather than relying on an old copy.
