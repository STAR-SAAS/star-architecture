# STAR Layered Memory and Context Loading

| Field | Value |
|---|---|
| Document ID | SWS-MEM-001 |
| Version / status | v0.1.1 — Working baseline; not frozen |
| Scope | STAR organizational memory and runtime context loading |

## 1. Principle

GitHub is STAR's durable structured organizational memory for material decisions, status, approved artifacts and traceable evidence. It is not a raw chat archive.

Synchronize material Confirmed decisions and supersession, concise Work Status, approved or reviewable artifacts, material validation evidence and handoffs. Exclude conversational noise, repetitions, abandoned drafts, raw transcripts by default, secrets and protected data.

## 2. Scope-level runtime package

Each active domain, product, Mission or material workstream should converge on:

```text
CONTEXT_PACKAGE.md              # entrypoint
ACTIVE_DECISIONS.md             # required payload
WORK_STATUS.md                  # required payload
DECISION_LOG.md                 # historical authority; conditional load
OPEN_QUESTIONS.md               # optional
HANDOFF.md                      # optional / transfer trigger
```

`CONTEXT_PACKAGE.md` contains pointers, classification and verification metadata. It is loaded once as the entrypoint and is not recursively reloaded as required payload.

## 3. Required and optional manifests

The Context Package declares required payload files, optional files, evidence triggers and file-level versions. Required payload loads by default. Optional files load only when the current task, lifecycle state, conflict or risk trigger requires them.

## 4. Active decisions and history

- `ACTIVE_DECISIONS.md` is a compact runtime projection of currently effective decisions.
- `DECISION_LOG.md` remains append-only historical authority, retaining Superseded decisions and provenance.
- Every active entry links to its Decision ID.
- Full history loads only for conflict, audit, supersession or provenance review.

## 5. Work Status as resume authority

`WORK_STATUS.md` is the primary resume record. It contains objective, primary lifecycle state, interrupt/prior state, verified completed work, current task, next actions, blockers, decision need, authoritative branch/commit/file metadata and latest Handoff. It must not become a chronological diary.

## 6. Progressive disclosure

```text
Global → Domain → Product / Mission → Task → Evidence
```

At each layer, load only the entrypoint and required payload needed to interpret the narrower layer. Evidence loads last and only for the active claim or action. Whole-repository, all-chat and full-history loading are never defaults.

## 7. File-level incremental loading

1. Resolve the Scope alias through the authoritative Alias Registry.
2. Read `CONTEXT_PACKAGE.md` once.
3. Compare recorded branch head, required-file blob SHAs and verification timestamps with the live source.
4. If branch head is unchanged, reuse the verified runtime package.
5. If branch head changed but required-file blobs are unchanged, the runtime package may remain Current.
6. If a required-file blob changed, load only the changed required file.
7. If optional or evidence files changed, load them only when their trigger applies.
8. A Context Package metadata-only change does not trigger a full reload.
9. Update verification metadata after a successful material review.

This file-level model prevents unrelated repository commits from forcing unnecessary context reload.

## 8. Classification and access

Every Context Package declares:

- classification: Public / Internal / Confidential / Restricted;
- repository visibility;
- permitted audience;
- whether a public summary is allowed;
- private authoritative source;
- redaction state;
- evidence access boundary;
- retention or review owner.

Public repositories contain safe summaries and pointers only. They must not expose employee permissions, customer or merchant facts, KYC/AML, payment data, incidents, commercial risk, credentials or private conversation content. Private operational detail remains in approved private systems.

SAIG retains authority for AI privacy, retention, employee-data, audit and AI-record controls. SWS defines the generic structure and routing boundary only.

## 9. Token budget

Token allocation is proportional to risk and available mode:

- Chat: entrypoint plus required payload and one evidence item at a time;
- Work: required payload plus selected optional records and bounded cross-source evidence;
- Codex: required payload plus task-relevant repository tree, diff, tests and CI state.

Preserve in order: scope and authority; active decisions; objective/next action/blockers; safety and data boundaries; evidence links; historical explanation.

Exact numeric budgets remain Candidate until pilot measurement.

## 10. Freshness

- **Current:** required-file fingerprints match live content or were freshly verified.
- **Stale:** required operational content exceeded its review trigger or changed without review.
- **Unverified:** live source could not be accessed or only secondary evidence was available.
- **Missing:** a required record, owner or alias does not exist.

A changed branch head alone does not make the runtime package Stale when required-file blobs are unchanged. Final time thresholds remain Candidate.

## 11. Mode transfer

Recommend or use the most suitable available mode based on dominant work. Seamless mode transfer and context inheritance are Candidate and environment-dependent. Where direct transfer is unavailable, preserve the existing Contract and create a Handoff; do not ask the user to repeat authoritative context.

## 12. Short-instruction resume

For `continue M001`:

1. resolve `M001` through the authoritative Alias Registry;
2. identify Mission-001, Project, professional conversation and repository;
3. load the entrypoint and verify file-level versions;
4. load Active Decisions and Work Status;
5. state objective, plan, blocker and decision need;
6. recommend or use Work/Codex according to the next action;
7. continue without asking for confirmed requirements again.

This path is conceptually validated and operationally Unverified until a controlled pilot succeeds.

## 13. Validation boundaries

- SAIG uses a private package and keeps sensitive permission/evidence detail private.
- M001 exposes confirmed requirements and current task state without loading historical discussion by default.
- Command Desk loads coordination state and links professional sources rather than importing professional detail.

## 14. Pilot measures

Track short-instruction success, files/tokens loaded, repeated context requests, stale detection, unnecessary history loads, missed synchronization, alias collisions, mode-transfer failures, and sensitive-data or authority-boundary failures.
