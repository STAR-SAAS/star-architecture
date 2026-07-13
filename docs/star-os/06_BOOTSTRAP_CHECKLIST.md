# STAR Conversation Bootstrap Checklist

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Confirmed working checklist; not frozen |
| **Scope** | Every new or resumed STAR conversation before material work |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | Inheritance failure, missing source, conflict or freeze proposal |
| **Authoritative working source** | This file in the active Draft PR; `main` only after approved merge |

## Checklist

| Check | Pass condition |
|---|---|
| **1. Workstream identified** | Global, domain, product, Mission or task scope is clear |
| **2. Global rules loaded** | `00_GLOBAL_WORKING_RULES.md` and `01_GLOBAL_DECISION_LOG.md` reviewed |
| **3. Workstream registered** | `04_WORKSTREAM_REGISTRY.md` identifies the workstream or records the missing source |
| **4. Local records loaded** | Applicable Charter, Decision Log, Open Questions, assumptions and Work Status reviewed |
| **5. Scope inheritance resolved** | Applicable Global → Domain → Product/Mission → Task rules are known |
| **6. Freshness checked** | Superseded, expired, unavailable or contradictory instructions are identified |
| **7. Sensitive boundary checked** | Public, internal, confidential and restricted information are routed correctly |
| **8. Current state summarized** | Objective, completed work, blockers, open questions and next task are known |
| **9. Reconfirmation test passed** | No previously confirmed decision is being presented as a new choice |
| **10. Decision gate checked** | User input is requested only for a genuine new decision, exception or missing authoritative fact |

## Result

Use one of three outcomes:

- **PASS** — continue work without asking the user to repeat prior decisions.
- **BLOCKED** — an authoritative source or factual input is missing; request only the smallest missing input.
- **EXCEPTION REQUIRED** — an applicable decision conflicts with the proposed work; cite the Decision ID and request the necessary accountable decision.

## Minimum audit note

For material work, record:

```text
Workstream:
Bootstrap date:
Applicable Global Decisions:
Applicable local Decisions:
Authoritative sources read:
Conflicts / missing sources:
Result: PASS / BLOCKED / EXCEPTION REQUIRED
User decision required now: Yes / No
Next task:
```

The checklist is complete only when the inherited context is actually used in the work, not merely when the files have been opened.
