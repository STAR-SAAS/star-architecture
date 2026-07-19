# SWS-001 · STAR Workspace Specification

| Field | Value |
|---|---|
| **Document ID** | SWS-001 |
| **Version / status** | v0.2.2 — Confirmed working baseline; not frozen; tooling-access baseline added |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-19 (Asia/Singapore) |
| **Review trigger** | Workspace architecture change, pilot finding, source-of-truth failure, context-loading failure, access-boundary change or freeze proposal |
| **Authoritative working source** | Draft PR #2 working branch; child Draft PR records become authoritative after merge into `agent/star-os-global-working-rules` |
| **Scope** | STAR OS platform-level workspace and conversation architecture |
| **Access** | Public architecture baseline; sensitive operational records remain in approved private systems |

## Purpose

SWS-001 defines STAR Workspace across Chat, Work, Codex, Projects, Memory, GitHub and future AI capabilities. It treats Workspace as scope-governed, record-backed and context-driven rather than binding the architecture permanently to one vendor interface.

## Current objective

Pilot the minimum STAR Command Center and STAR Conversation Governance while preserving professional execution and detailed truth in owning Projects, repositories and systems.

## Architecture direction

The working object model uses Scope, Actor, Capability, Activity, Record, Context Package and Typed Relationship.

Runtime context follows:

```text
Global → Domain → Product / Mission → Task → Evidence
```

GitHub is durable structured memory, not a raw chat archive. `CONTEXT_PACKAGE.md` is an entrypoint; `ACTIVE_DECISIONS.md` and concise `WORK_STATUS.md` are required payload. Full history and evidence load only on trigger.

## Lifecycle direction

Primary path:

```text
Intake → Routed → Bootstrapped → Active → Review → Closed
```

Waiting and Blocked are interrupt states with recorded recovery to the prior state. Transfer starts the receiver at Bootstrapped and ends the sender's active ownership. Closed is not silently reopened.

## Command Center boundary

`STAR Command Center` contains only `⭐ STAR Command Desk` during the pilot. Command Desk performs intake, priority, routing, portfolio coordination, blocker and decision visibility, report-back verification and concise feedback. Professional work remains in the relevant professional conversation.

## Authoritative and working records

### Core SWS records

1. [`01_DECISION_LOG.md`](01_DECISION_LOG.md)
2. [`02_OPEN_QUESTIONS_AND_MISSING_EVIDENCE.md`](02_OPEN_QUESTIONS_AND_MISSING_EVIDENCE.md)
3. [`03_WORK_STATUS.md`](03_WORK_STATUS.md)
4. [`04_COMMAND_CENTER_MINIMUM_LAUNCH_SPECIFICATION.md`](04_COMMAND_CENTER_MINIMUM_LAUNCH_SPECIFICATION.md)
5. [`command-center/STAR-PORTFOLIO-STATUS.md`](command-center/STAR-PORTFOLIO-STATUS.md)
6. [`GIT_GITHUB_CODEX_ACCESS_BASELINE.md`](GIT_GITHUB_CODEX_ACCESS_BASELINE.md)

### Conversation governance

7. [`STAR_CONVERSATION_GOVERNANCE.md`](STAR_CONVERSATION_GOVERNANCE.md)
8. [`STAR_CONVERSATION_CONTRACT_TEMPLATE.md`](STAR_CONVERSATION_CONTRACT_TEMPLATE.md)
9. [`STAR_CONVERSATION_ROUTING_MATRIX.md`](STAR_CONVERSATION_ROUTING_MATRIX.md)
10. [`STAR_CHAT_WORK_CODEX_MODE_SELECTION.md`](STAR_CHAT_WORK_CODEX_MODE_SELECTION.md)
11. [`STAR_LAYERED_MEMORY_AND_CONTEXT_LOADING.md`](STAR_LAYERED_MEMORY_AND_CONTEXT_LOADING.md)
12. [`STAR_CONTEXT_PACKAGE_TEMPLATE.md`](STAR_CONTEXT_PACKAGE_TEMPLATE.md)

## Authority and data model

- Child PR content becomes part of the Draft PR #2 working baseline only after merge into `agent/star-os-global-working-rules`.
- The portfolio ledger is authoritative only for portfolio coordination.
- Professional truth remains in the relevant professional authoritative source.
- Public repositories contain safe summaries and pointers only.
- SAIG retains authority for AI privacy, retention, employee-data, audit and AI-record controls.
- Chat history and AI memory are working context, not durable organizational authority.
- Tooling access evidence records current capability only and never grants change authority.

## Current state

- Minimum Command Center architecture: confirmed working direction.
- Conversation-governance baseline: revised working baseline; not frozen.
- Decision-history correction: SWS-DEC-014 added while preserving SWS-DEC-006.
- Layered memory: file-level fingerprint design added; operational pilot incomplete.
- Direct mode transfer: Candidate / environment-dependent.
- Scope Alias Registry: Missing; open question recorded.
- `continue M001`: conceptually validated / operationally Unverified.
- Command Center Portfolio Ledger: calibrated through DSP-001-028 publication; future material changes still require verification.
- Git / GitHub / Codex access baseline: recorded with separate user-verified local evidence and connector-verified cloud evidence.
- No existing conversations are created, migrated or deleted by this work.
