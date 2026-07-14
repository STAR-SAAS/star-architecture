# SWS-001 · STAR Workspace Specification

| Field | Value |
|---|---|
| **Document ID** | SWS-001 |
| **Version / status** | v0.1.0 — Confirmed working baseline; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-14 (Asia/Singapore) |
| **Review trigger** | Workspace architecture change, pilot finding, scope conflict, source-of-truth failure or freeze proposal |
| **Authoritative working source** | `STARSAAS/star-architecture`, Draft PR #2, branch `agent/star-os-global-working-rules` |
| **Scope** | STAR OS platform-level workspace information architecture |
| **Access** | Public architecture baseline; sensitive operational records remain in approved private systems |

## Purpose

SWS-001 defines the long-term information architecture of STAR Workspace across Chat, Work, Codex, Projects, Memory, Knowledge Base, GitHub and future AI capabilities.

It is a STAR OS platform-level architecture specification. It is not a product requirements document and does not make any current vendor interface the permanent architecture.

## Current objective

Establish and pilot the minimum STAR Command Center as the cross-project orchestration layer while preserving professional execution and authoritative records in their corresponding Projects, repositories and systems.

## Current architecture direction

STAR Workspace is treated as a scope-governed, record-backed and context-driven platform.

The current working object model uses:

1. Scope;
2. Actor;
3. Capability;
4. Activity;
5. Record;
6. Context Package;
7. Typed Relationship as a structural primitive.

These are confirmed working directions, not frozen architecture.

## Command Center boundary

STAR Command Center is a separate Project whose initial version contains only one Chat: `⭐ STAR Command Desk`.

Command Desk is limited to:

- intake;
- prioritization;
- routing;
- portfolio-level status tracking;
- blocker, dependency and decision-needed visibility;
- receiving report-backs;
- updating the portfolio ledger;
- concise feedback.

Professional work remains in the relevant Project and professional conversation.

## Authoritative records

1. [`01_DECISION_LOG.md`](01_DECISION_LOG.md)
2. [`02_OPEN_QUESTIONS_AND_MISSING_EVIDENCE.md`](02_OPEN_QUESTIONS_AND_MISSING_EVIDENCE.md)
3. [`03_WORK_STATUS.md`](03_WORK_STATUS.md)
4. [`04_COMMAND_CENTER_MINIMUM_LAUNCH_SPECIFICATION.md`](04_COMMAND_CENTER_MINIMUM_LAUNCH_SPECIFICATION.md)
5. [`command-center/STAR-PORTFOLIO-STATUS.md`](command-center/STAR-PORTFOLIO-STATUS.md)

## Authority model

- This directory is authoritative for the current SWS-001 working baseline.
- `STAR-PORTFOLIO-STATUS.md` is authoritative only for portfolio coordination status.
- Detailed architecture, governance, product, code, test and operational truth remains in the relevant professional authoritative source.
- Chat history and AI memory are working context, not durable organizational authority.

## Current state

- Minimum Command Center architecture: confirmed working direction.
- `STAR Command Center` Project: reported created by the user.
- `⭐ STAR Command Desk`: reported created by the user.
- Portfolio ledger: created in this Draft PR by the SWS-001 authority-establishment task.
- Initial three portfolio items: placeholders requiring professional-source verification before pilot activation.
- SWS-001: active and incomplete; not approved or frozen.
