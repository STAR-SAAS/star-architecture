# SWS-001 · Open Questions and Missing Evidence

| Field | Value |
|---|---|
| **Version / status** | v0.2.0 — Active |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 plus DSP-001-004 working branch until approved merge |
| **Scope** | SWS-001, STAR Command Center pilot and conversation-governance pilot |

Open questions and missing evidence must not be presented as confirmed architecture or verified operational state.

## Priority A — required pilot evidence

| ID | Question or missing evidence | State | Required next evidence |
|---|---|---|---|
| **SWS-OQ-001** | Are the final STAR Command Center Project Instructions installed exactly enough to enforce orchestration-only behavior? | Missing | Compare installed Project Instructions with SWS-CC-001. |
| **SWS-OQ-002** | What is the verified current professional status and owner of each pilot workstream? | Partially verified; must remain source-linked | Load current Context Package / Decision Log / Work Status for SWS, SAIG and M001. |
| **SWS-OQ-004** | Can Command Desk maintain the portfolio ledger reliably? | Evidence exists from real dispatch cycles; final pilot assessment pending | Record verified commits and failures across more than one cycle. |
| **SWS-OQ-010** | Where will each pilot Scope place its canonical `CONTEXT_PACKAGE.md`, `ACTIVE_DECISIONS.md` and `WORK_STATUS.md`? | Candidate structure; implementation Missing | Implement and review packages in SAIG, M001 and Command Desk scopes. |
| **SWS-OQ-011** | Can `continue M001` reliably resolve the correct Scope, conversation, branch and runtime package without user reconstruction? | Unverified | Run a controlled resume test and record files loaded, token/file footprint and result. |

## Priority B — usability and efficiency validation

| ID | Question or missing evidence | Validation approach |
|---|---|---|
| **SWS-OQ-005** | Does the Dispatch package provide enough context without duplicating professional history? | Compare real dispatches across SWS, SAIG and M001. |
| **SWS-OQ-006** | Is Report Back concise and complete enough to update durable status? | Compare actual report-backs and ledger updates. |
| **SWS-OQ-007** | What makes a Scope Current, Stale or Unverified? | Observe change cadence before fixing thresholds. |
| **SWS-OQ-008** | Does one Command Desk remain sufficient? | Record actual overload, routing failure or access conflict. |
| **SWS-OQ-009** | Is the public architecture repository appropriate for each coordination record? | Classify real entries; keep sensitive detail in private sources. |
| **SWS-OQ-012** | What token/file budgets are safe and useful for Chat, Work and Codex? | Measure required and optional loads during the three pilots. |
| **SWS-OQ-013** | Should context packages be manually maintained, generated, or hybrid? | Pilot manual packages before proposing automation. |

## Confirmed matters not to reopen without new evidence

- Correct Project and professional conversation are stated proactively.
- Brief warnings are used for Chat / Work / Codex mismatch.
- Users are not asked to repeat decisions available in authoritative records.
- GitHub stores durable structured memory, not raw chat archives.
- Runtime loading is progressive and incremental; whole-repository and full-history loading are not default.
- No existing conversations are migrated or deleted by this baseline.
- The baseline is not frozen.

## Deferred broader work

- complete Activity and Work Model;
- automated context-package generation and synchronization;
- future Agent orchestration;
- final role-specific Workspace views;
- full Memory and Knowledge lifecycle beyond the current structured-memory baseline.
