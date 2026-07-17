# SWS-001 · Open Questions and Missing Evidence

| Field | Value |
|---|---|
| **Version / status** | v0.2.1 — Active |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 plus PR #3 proposed record version until approved merge |
| **Scope** | SWS-001, STAR Command Center pilot and conversation-governance pilot |

Open questions and missing evidence must not be presented as confirmed architecture or verified operational state. Prior Question IDs remain visible when closed, superseded or reformulated.

## Priority A — required pilot evidence

| ID | Question or missing evidence | State | Required next evidence |
|---|---|---|---|
| **SWS-OQ-001** | Are final STAR Command Center Project Instructions installed closely enough to enforce orchestration-only behavior? | Missing | Compare installed Project Instructions with SWS-CC-001. |
| **SWS-OQ-002** | What is the verified current professional status and owner of each pilot workstream? | Partially verified; source-linked refresh required | Load current Context Package / Decision Log / Work Status for SWS, SAIG and M001. |
| **SWS-OQ-004** | Can Command Desk maintain the portfolio ledger reliably? | Partial evidence; portfolio ledger currently Stale / update pending | Record verified commits and failures across more than one safe update cycle. |
| **SWS-OQ-010** | Where will each pilot Scope place its canonical Context Package, Active Decisions and Work Status? | Candidate structure; implementation Missing | Implement and review packages in SAIG, M001 and Command Desk scopes. |
| **SWS-OQ-011** | Can `continue M001` resolve the correct Scope, conversation, branch and runtime package without user reconstruction? | Conceptually validated / operationally Unverified | Run a controlled resume test and record files loaded, token/file footprint and result. |
| **SWS-OQ-014** | Where is the authoritative Scope Alias Registry? | Missing | Decide canonical file location, alias uniqueness, collision handling, migration updates and deprecated-alias retention. |
| **SWS-OQ-015** | Are classification, audience, redaction and evidence-access fields sufficient across public and private Context Packages? | Candidate | Validate one public SWS/Command Desk package and one private SAIG package without exposing protected data. |

## Priority B — usability and efficiency validation

| ID | Question or missing evidence | Validation approach |
|---|---|---|
| **SWS-OQ-005** | Does the Dispatch package provide enough context without duplicating professional history? | Compare real dispatches across SWS, SAIG and M001. |
| **SWS-OQ-006** | Is Report Back concise and complete enough to update durable status? | Compare actual report-backs and ledger updates. |
| **SWS-OQ-007** | What makes a Scope Current, Stale or Unverified? | Test file-level fingerprints and observe operational cadence before fixing time thresholds. |
| **SWS-OQ-008** | Does one Command Desk remain sufficient? | Record actual overload, routing failure or access conflict. |
| **SWS-OQ-009** | Is the public architecture repository appropriate for each coordination record? | Classify real entries; retain sensitive detail in private sources. |
| **SWS-OQ-012** | What token/file budgets are safe and useful for Chat, Work and Codex? | Measure entrypoint, required payload, optional and evidence loads during pilots. |
| **SWS-OQ-013** | Should Context Packages be manually maintained, generated or hybrid? | Pilot manual packages before proposing automation. |
| **SWS-OQ-016** | Which environments support direct mode transfer and seamless Contract/context inheritance? | Record actual platform behavior; use Handoff when unavailable. |
| **SWS-OQ-017** | Should Closed work ever use a governed Reopened state? | Observe pilot needs; until decided, use a new Activity / Contract. |

## Closed / Superseded Questions

| ID | Closure status | Closure basis | Evidence | Closure date | Replacement question |
|---|---|---|---|---|---|
| **SWS-OQ-003** | Closed for minimum pilot; ownership detail remains source-specific | Named ownership is required by the Contract and Context Package; absent owners remain Missing rather than blocking the generic model | SWS-DEC-010 and Contract/Context Package fields in PR #3 | 2026-07-17 | SWS-OQ-002 continues verification of actual pilot owners |

No other prior Question ID is closed or deleted by this revision.

## Confirmed matters not to reopen without new evidence

- Correct Project and professional conversation are stated proactively.
- Brief warnings are used for mode mismatch.
- Users are not asked to repeat decisions available in authoritative records.
- GitHub stores durable structured memory, not raw chat archives.
- Runtime loading is progressive and file-level incremental; whole-repository and full-history loading are not default.
- No existing conversations are migrated or deleted by this baseline.
- The baseline is not frozen.
- SAIG retains authority for AI privacy, retention, employee-data, audit and AI-record controls.

## Deferred broader work

- complete Activity and Work Model;
- automatic Context Package generation and synchronization;
- future Agent orchestration;
- final role-specific Workspace views;
- full Memory and Knowledge lifecycle beyond the current structured-memory baseline.
