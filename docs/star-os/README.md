# STAR OS Global Governance

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Working baseline; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | Global rule change, new domain, cross-conversation conflict, governance incident or freeze proposal |
| **Authoritative working source** | This repository path in its Draft PR; `main` only after approved merge |
| **Access** | Public; employee, account, customer and sensitive governance records belong in an approved private system |

## Purpose

This directory contains the rules that must survive across STAR conversations, domains, products, Missions and AI tools.

A rule is not reliably governed merely because it appeared in an earlier chat. Cross-cutting rules must be recorded here, given an explicit scope and loaded through the conversation bootstrap protocol.

## Start here

1. [`STAR_OS_GLOBAL_WORKING_RULES.md`](STAR_OS_GLOBAL_WORKING_RULES.md) — confirmed cross-cutting working disciplines.
2. [`STAR_CONVERSATION_BOOTSTRAP_PROTOCOL.md`](STAR_CONVERSATION_BOOTSTRAP_PROTOCOL.md) — how every new STAR conversation inherits the right context.
3. [`STAR_DECISION_SCOPE_AND_PROPAGATION.md`](STAR_DECISION_SCOPE_AND_PROPAGATION.md) — where a decision applies and how it is propagated.
4. [`STAR_GLOBAL_DECISION_LOG.md`](STAR_GLOBAL_DECISION_LOG.md) — confirmed global decisions.
5. [`STAR_CONVERSATION_HANDOFF_TEMPLATE.md`](STAR_CONVERSATION_HANDOFF_TEMPLATE.md) — minimum handoff package for moving or resuming work.
6. [`CHANGELOG.md`](CHANGELOG.md) — chronological changes.

## Governing principle

> Chat is a working interface. Versioned, scoped and reviewed records are the durable organizational memory.

## Scope model

```text
STAR Global
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

Lower levels may add detail, but they must not silently contradict higher-level rules. An exception requires an explicit owner, reason, scope, expiry and approval.

## New-conversation rule

A new STAR conversation must not begin by asking the user to restate established global rules. It must first load the global rules, relevant domain records, current decisions and work status, then identify only the genuinely missing facts.
