# STAR Pre-Development Architecture Program (PDAP) — Founder-led Fast Track

| Field | Value |
|---|---|
| Status | Leadership Confirmed; not frozen |
| Accountable owner / decision approver | Jason Lin |
| Default executor | Jason Lin with approved AI capabilities |
| Professional conversation | 📚 STAR Architecture Framework (SAF) |
| Scope | Shared Foundation, SmartQuote and GateHub readiness |

## 1. Objective

Create sufficient, verified and time-boxed architecture and engineering readiness so Shared Foundation, SmartQuote and GateHub can begin safely without waiting for every reversible detail to be finalized.

Approved target starts:

- PDAP Phase 0: 2026-07-20
- Shared Foundation engineering: 2026-07-27
- SmartQuote formal development: 2026-08-03
- GateHub formal development: 2026-08-10

These are target dates, not automatic authorization, Gate passage or Commitment.

## 2. Founder-led operating model

Jason Lin and approved AI capabilities perform the default pre-development work. Another employee or specialist participates only when:

1. a clearly defined question cannot be completed safely by Jason and AI;
2. professional feasibility validation is mandatory; or
3. legal, compliance, security, financial, operational or technical authority is required.

Before participation, record the exact question, reason, expected evidence, named specialist, response deadline, blocking status and fallback or recovery path. Participation is minimum-necessary and does not transfer accountability.

Dorden reviews PDAP governance and final Exact Head publication integrity only. Dorden is not the sole product, architecture, security, testing or technical authority. Allen enters execution coordination only after explicit Product Commitment and Delivery start.

## 3. Phases

| Phase | Name | Outcome |
|---|---|---|
| 0 | Authority and Evidence Baseline | Verified sources, owners, freshness, conflicts, Missing and blocker candidates |
| 1 | Shared Constraints Framing | Company/shared boundaries, data ownership and Identity/Tenant/Security directions |
| 2 | Shared Foundation Readiness | Evidence for the Shared Foundation engineering-start Gate |
| 3 | SmartQuote Architecture Readiness | Minimum architecture package and readiness disposition |
| 4 | GateHub Architecture Readiness | Minimum architecture package and readiness disposition |
| 5 | Cross-product Review | Disposition of material overlaps and conflicts |
| 6 | Product Commitment / Delivery Start | Explicit Commit, Hold or Recovery decision per product |
| 7 | Transition and Controlled Follow-through | Delivery handoff; reversible matters move to ADR/RFC |

Phases may overlap when evidence permits, but applicable Gates may not be bypassed.

## 4. Blocking decisions

Only these classes may block a target date:

- high-cost and difficult-to-reverse decisions;
- cross-product architecture conflict;
- core data ownership;
- Identity, Tenant or Security boundaries;
- legal, compliance or material risk;
- technical questions that cannot advance safely through an Approved Assumption.

Reversible uncertainty does not block a target solely because it remains unresolved when an Approved Assumption records owner, scope, risk, validation trigger, review or expiry date and reversal path, and no applicable Gate blocker remains. It may instead enter an ADR or RFC backlog.

## 5. Controlled Spike

A Spike is bounded evidence-generation work. It does not constitute formal development, Product Commitment, Delivery start, production readiness or approval of production architecture. It must have a question, timebox, owner, evidence output and disposition.

## 6. Delay and recovery

A delay request must record:

```yaml
blocked_target:
blocker:
blocking_class:
owner:
decision_due_date:
closure_date:
recovery_plan:
revised_target_date:
approved_by:
```

A delay without these fields is not authoritative.

## 7. Dispatch control

Every PDAP Dispatch must identify:

```yaml
dispatch_id:
portfolio_item:
PDAP_phase:
readiness_gate:
objective:
scope:
non_goals:
accountable_owner:
decision_approver:
primary_executor:
specialist_required:
specialist_question:
approved_target_date:
timebox:
entry_conditions:
required_evidence:
blocking_decisions:
approved_assumptions:
allowed_work:
prohibited_work:
authoritative_sources:
required_report_back:
delay_recovery_fields:
```

A task that does not map to a valid Phase and Gate, or attempts to bypass a Gate, stops and returns to STAR Command Desk.

## 8. Non-authorizations

This program does not itself select or freeze a technology stack, approve product architecture, pass M1, commit M001, start Shared Foundation engineering, start SmartQuote Delivery, start GateHub Delivery, alter repository permissions or merge parent Draft PRs.
