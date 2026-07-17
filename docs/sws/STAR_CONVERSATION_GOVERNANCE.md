# STAR Conversation Governance

| Field | Value |
|---|---|
| Document ID | SWS-CG-001 |
| Version / status | v0.1.1 — Working baseline; not frozen |
| Owner | STAR leadership |
| Maintainer | STAR Architecture maintainers |
| Scope | All STAR conversations, Projects and supported AI modes |
| Decision references | GWR-01–12; SWS-DEC-005–014 |
| Record authority | Leadership-confirmed basis; PR #3 is a proposed record version until merged into Draft PR #2 |

## 1. Authority and ownership

This baseline adds operational detail to the Global Working Rules and does not override them. Every material conversation declares its Project, professional conversation, Scope/Activity ID, objective, accountable human owner, authoritative sources, available mode, lifecycle state and escalation boundary. Command Desk remains orchestration-only. Professional authority remains in professional Projects, authoritative records and named humans.

## 2. Conversation Contract and Routing Gate

Create a Contract once at conversation start. Reuse it on normal resume; refresh metadata or `WORK_STATUS.md` when sufficient. Create a new Contract only after a material Scope, owner, authority or completion-boundary change.

Before material work determine the correct Project, professional conversation, available mode, orchestration/professional boundary, authoritative Scope and decision need. Outcomes are Proceed, Proceed with brief warning, Route or Pause. Warnings stay brief and do not interrupt reversible work unnecessarily.

## 3. Bootstrap and runtime loading

Use progressive disclosure:

```text
Global → Domain → Product / Mission → Task → Evidence
```

Load `CONTEXT_PACKAGE.md` once as the entrypoint, then `ACTIVE_DECISIONS.md` and concise `WORK_STATUS.md`. Optional records and evidence load only on trigger. Do not load the whole repository, full chat history or full Decision Log by default. Do not ask the user to repeat authoritative decisions.

## 4. Lifecycle

Primary path:

```text
Intake → Routed → Bootstrapped → Active → Review → Closed
```

Waiting and Blocked are interrupt states available from Routed, Bootstrapped, Active or Review. Record `prior_state` before interruption. Waiting returns to the prior state when awaited input arrives. Blocked returns after blocker resolution.

Transferred is a handoff outcome outside the primary path: the receiver begins at Bootstrapped; the sender records Transferred and no longer owns active execution. Closed is not silently reopened. New work after closure uses a new Activity / Contract unless a future governed Reopened rule is approved.

## 5. Mode selection

Recommend or use the most suitable available Chat, Work or Codex mode according to dominant work. Mode never changes authority or source of truth. Direct mode switching and seamless context inheritance are Candidate and environment-dependent. Where unavailable, preserve the Contract and create a Handoff.

## 6. Durable memory responsibilities

- `DECISION_LOG.md`: append-only historical authority, provenance and supersession.
- `ACTIVE_DECISIONS.md`: concise projection of currently effective decisions.
- `WORK_STATUS.md`: primary task-resume record, not a chronological diary.
- `HANDOFF.md`: unfinished state across conversation, owner or tool changes.
- `CONTEXT_PACKAGE.md`: entrypoint, manifests, classification and verification metadata.

Candidate, Confirmed, Frozen, Superseded, Missing, Stale and Unverified remain distinct. Existing Decision IDs are not silently rewritten.

## 7. File-level freshness

Each Context Package records branch head and required-file blob SHAs/timestamps.

1. Branch unchanged: reuse the verified runtime package.
2. Branch changed but required-file blobs unchanged: package may remain Current.
3. Required-file blob changed: load only that changed required file.
4. Optional/evidence change: load only when its trigger applies.
5. Context metadata-only changes do not trigger a full reload.

Operational facts that cannot be verified are Stale or Unverified. Time thresholds remain Candidate pending pilot evidence.

## 8. Classification and sensitive data

Every Context Package declares classification, repository visibility, permitted audience, public-summary permission, private authoritative source, redaction status, evidence-access boundary and retention/review owner.

Public repositories contain safe summaries and pointers only. They must not expose employee permissions, customer or merchant facts, KYC/AML, payment data, incidents, commercial risk, credentials or private conversation content. Private operational detail remains in approved private sources.

SAIG retains authority for AI privacy, retention, employee-data, audit and AI-record controls. SWS defines only the generic structure and routing boundary.

## 9. Short-instruction resume

`continue M001` should resolve the authoritative alias, identify Mission-001 and its professional location, load the entrypoint and changed required payload, state objective/plan/blocker/decision need, and recommend or use the available mode. It is conceptually validated and operationally Unverified until pilot evidence exists. If alias resolution fails, search the authoritative Alias Registry and indexes before asking the user.

## 10. Interruption, escalation and closure

Continue reversible in-scope work in batches. Pause for strategy/scope/authority changes, Decision-ID changes, material customer/security/compliance/financial/operational risk, difficult-to-reverse architecture, rollout/migration/deletion/external commitment, or leadership preference between valid alternatives.

A conversation closes only when the outcome is complete, material records are synchronized, remaining work is transferred or recorded, and the STAR Self-Review Gate passes.

## 11. Failure handling

- Missing: record fact, owner, impact and required evidence; never invent.
- Stale: verify the live source or retain the dated last-known value.
- Unverified: secondary evidence cannot prove current state, approval or completion.
- Conflict: apply Scope hierarchy, Decision IDs and provenance.
- Tool failure: preserve last verified state, avoid duplicate writes and provide a safe manual path.

## 12. Validation and pilot boundary

- SAIG: private package; sensitive evidence stays private; policy, Wave A and pilot authorization remain separate.
- M001: confirmed requirements load without re-asking; implementation evidence loads only when needed.
- Command Desk: coordination package and ledger only; links professional sources and does not perform professional execution.

Pilot only across SWS/SAF, SAIG, M001 and Command Desk. Measure routing accuracy, short-resume success, files/tokens loaded, stale detection, mode-transfer failures, handoff quality and sensitive-data boundary failures. Do not freeze, broadly roll out or activate automatic synchronization without later evidence and approval.
