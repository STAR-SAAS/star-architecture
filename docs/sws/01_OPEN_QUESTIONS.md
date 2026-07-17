# SWS-001 · Open Questions and Missing Evidence

| Field | Value |
|---|---|
| **Version / status** | v0.2.2 — Active |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 working branch plus approved child Draft PR record version until merged |
| **Scope** | SWS-001, STAR Command Center pilot and conversation-governance pilot |

Open questions and missing evidence must not be presented as confirmed architecture or verified operational state. Prior Question IDs remain visible when closed, superseded or reformulated.

## Priority A — required pilot evidence

| ID | Question or missing evidence | State | Required next evidence |
|---|---|---|---|
| **SWS-OQ-001** | Are final STAR Command Center Project Instructions installed closely enough to enforce orchestration-only behavior? | Missing | Compare installed Project Instructions with SWS-CC-001. |
| **SWS-OQ-002** | What is the verified current professional status and owner of each pilot workstream? | Leadership-approved role matrices recorded; startup evidence still incomplete | Verify Package-specific access, locations, authority and execution readiness against SWS-DEC-015. |
| **SWS-OQ-004** | Can Command Desk maintain the portfolio ledger reliably? | Partial evidence; portfolio ledger currently Stale / update pending | Execute the approved Safe Ledger Update method on one Portfolio Item and preserve exact commit/blob, full readback, diff, recovery point and independent review evidence. |
| **SWS-OQ-010** | Where will each pilot Scope place its canonical Context Package, Active Decisions and Work Status? | Pilot Candidate paths approved; files not created | Package A exact private directory remains Missing; Package B and C candidate paths are approved under SWS-DEC-015 but require implementation and review. |
| **SWS-OQ-011** | Can `continue M001` resolve the correct Scope, conversation, branch and runtime package without user reconstruction? | Conceptually validated / operationally Unverified | Confirm Alias authority and execution authorization, create approved files in a later authorized task, then run a controlled resume test. |
| **SWS-OQ-014** | Where is the authoritative Scope Alias Registry? | Pilot Candidate path approved; authority Missing | Validate `docs/sws/PILOT_ALIAS_REGISTRY.md` only as a Pilot Candidate; confirm Alias owner, write authority and modification approval before creation. |
| **SWS-OQ-015** | Are classification, audience, redaction and evidence-access fields sufficient across public and private Context Packages? | Candidate; Package A boundary approved but not implemented | Validate one public SWS/Command Desk package and one Internal-only SAIG package without exposing protected data. |

## Package-specific Remaining Missing under SWS-DEC-015

### Package A — SAIG

- exact private Context Package directory;
- Allen Liao and related-role actual access verification;
- authorized submitting maintainer;
- opaque `public_reference_id` and controlled private mapping;
- final retention and review implementation;
- private-source access test.

### Package B — M001

- Alias owner;
- write authority;
- Alias modification approval workflow;
- Context Package files and Pilot Alias Registry do not yet exist;
- required-file fingerprints;
- actual resume-test environment and execution authorization.

### Package C — Command Desk

- Context Package files do not yet exist;
- actual execution tools and permission verification;
- write-time Ledger commit and blob SHA;
- exact professional Report Back selected for the end-to-end test;
- Safe Ledger Update demonstration and independent-review evidence.

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
- SWS-DEC-015 approves startup conditions only; it does not start a Package or create its files.

## Deferred broader work

- complete Activity and Work Model;
- automatic Context Package generation and synchronization;
- future Agent orchestration;
- final role-specific Workspace views;
- full Memory and Knowledge lifecycle beyond the current structured-memory baseline.