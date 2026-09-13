# STAR Conversation Bootstrap Protocol

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Confirmed working protocol; not frozen |
| **Scope** | Every new or resumed STAR conversation |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | Failed inheritance, new workstream, source-location change, conflict or freeze proposal |
| **Authoritative working source** | This file in the active Draft PR; `main` only after approved merge |

## Objective

Start work with inherited, current and scoped context so the user does not need to repeat previously confirmed decisions.

## Bootstrap sequence

Before material work in a new or resumed conversation:

1. **Identify the workstream** — Global, domain, product, project, Mission or temporary task.
2. **Read global governance** — Global Working Rules and Global Decision Log.
3. **Read the workstream registry** — locate the authoritative domain/project records.
4. **Read applicable local records** — Charter, Decision Log, Open Questions, Assumptions, Work Status and current Mission/Task record.
5. **Apply the propagation model** — determine which global and parent decisions apply.
6. **Check conflicts and freshness** — identify superseded, expired, missing or contradictory instructions.
7. **Build a compact inherited-context summary** — confirmed rules, current candidates, open questions, blockers and next task.
8. **Continue without reconfirmation** — do not ask the user to approve decisions already confirmed within scope.
9. **Escalate only genuine deltas** — cite Decision IDs when a change, exception or new executive choice is required.
10. **Update durable records** — record any new confirmed decision, status change or conflict before ending the batch.

## Minimum inherited-context summary

A new conversation should internally establish:

```text
Workstream:
Authoritative source:
Applicable global decisions:
Applicable domain/project/Mission decisions:
Current objective:
Current status:
Open questions:
Known blockers:
Next evidence-producing task:
User decision required now: Yes / No
```

This summary does not need to be shown in full unless it helps the user. It must guide the work.

## Do not ask again

Do not ask the user to reconfirm:

- writing and reporting preferences already recorded globally;
- confirmed repository locations or workstream boundaries;
- confirmed review, Markdown, validation or stakeholder rules;
- domain or Mission decisions that still apply and have not been superseded.

## Ask again only with a cited reason

A new confirmation request must state:

1. the existing Decision ID;
2. the current decision;
3. what changed;
4. why the old decision is no longer sufficient;
5. the options and impacts now requiring a decision.

## Missing access or missing record

When the authoritative record cannot be accessed:

- state that the record is unavailable;
- do not invent its contents;
- use any safely available confirmed context;
- request the smallest factual input needed only when work cannot proceed;
- once access is restored, reconcile and update the record.
