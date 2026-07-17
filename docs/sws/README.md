# SWS-001 · STAR Workspace Specification

| Field | Value |
|---|---|
| **Document ID** | SWS-001 |
| **Version / status** | v0.2.0 — Confirmed working baseline; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Review trigger** | Workspace architecture change, pilot finding, source-of-truth failure, context-loading failure or freeze proposal |
| **Authoritative working source** | Draft PR #2 plus approved SWS working branches until merged |
| **Scope** | STAR OS platform-level workspace and conversation architecture |
| **Access** | Public architecture baseline; sensitive operational records remain in approved private systems |

## Purpose

SWS-001 defines STAR Workspace across Chat, Work, Codex, Projects, Memory, GitHub and future AI capabilities. It treats Workspace as scope-governed, record-backed and context-driven rather than permanently binding the architecture to one vendor interface.

## Current objective

Pilot the minimum STAR Command Center and STAR Conversation Governance while preserving professional execution and detailed truth in their owning Projects, repositories and systems.

## Architecture direction

The current working object model uses Scope, Actor, Capability, Activity, Record, Context Package and Typed Relationship.

Conversation runtime follows:

```text
Global → Domain → Product / Mission → Task → Evidence
```

GitHub is durable structured memory, not a raw chat archive. Scope-level context packages provide low-token runtime entry points.

## Command Center boundary

`STAR Command Center` contains only `⭐ STAR Command Desk` during the pilot. Command Desk performs intake, priority, routing, portfolio coordination, blocker and decision visibility, report-back verification and concise feedback. Professional work remains in the relevant professional conversation.

## Authoritative and working records

### Core SWS records

1. [`01_DECISION_LOG.md`](01_DECISION_LOG.md)
2. [`02_OPEN_QUESTIONS_AND_MISSING_EVIDENCE.md`](02_OPEN_QUESTIONS_AND_MISSING_EVIDENCE.md)
3. [`03_WORK_STATUS.md`](03_WORK_STATUS.md)
4. [`04_COMMAND_CENTER_MINIMUM_LAUNCH_SPECIFICATION.md`](04_COMMAND_CENTER_MINIMUM_LAUNCH_SPECIFICATION.md)
5. [`command-center/STAR-PORTFOLIO-STATUS.md`](command-center/STAR-PORTFOLIO-STATUS.md)

### Conversation governance

6. [`STAR_CONVERSATION_GOVERNANCE.md`](STAR_CONVERSATION_GOVERNANCE.md)
7. [`STAR_CONVERSATION_CONTRACT_TEMPLATE.md`](STAR_CONVERSATION_CONTRACT_TEMPLATE.md)
8. [`STAR_CONVERSATION_ROUTING_MATRIX.md`](STAR_CONVERSATION_ROUTING_MATRIX.md)
9. [`STAR_CHAT_WORK_CODEX_MODE_SELECTION.md`](STAR_CHAT_WORK_CODEX_MODE_SELECTION.md)
10. [`STAR_LAYERED_MEMORY_AND_CONTEXT_LOADING.md`](STAR_LAYERED_MEMORY_AND_CONTEXT_LOADING.md)
11. [`STAR_CONTEXT_PACKAGE_TEMPLATE.md`](STAR_CONTEXT_PACKAGE_TEMPLATE.md)

## Authority model

- This directory is authoritative for the current SWS-001 working baseline only after the applicable reviewed version is merged.
- The portfolio ledger is authoritative only for portfolio coordination.
- Detailed architecture, governance, product, code, test and operational truth remains in the relevant professional authoritative source.
- Chat history and AI memory are working context, not durable organizational authority.
- Active decisions and concise Work Status should load by default; full history and evidence load progressively.

## Current state

- Minimum Command Center architecture: confirmed working direction.
- Conversation-governance baseline: prepared for review; not frozen.
- Layered GitHub memory and incremental context loading: confirmed working direction; pilot implementation incomplete.
- Short-instruction resume such as `continue M001`: designed but not yet validated against live runtime packages.
- No existing conversations are migrated or deleted by this work.
