# SWS-001 · Open Questions and Missing Evidence

| Field | Value |
|---|---|
| **Version / status** | v0.3.0 — Active Pilot questions |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-21 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 working branch |
| **Scope** | SWS-001, STAR Command Center pilot and conversation-governance pilot |

Open questions and missing evidence must not be presented as confirmed architecture or verified operational state. Historical detail belongs in the Decision Log, Changelog, Portfolio Ledger or owning professional source rather than this current-question register.

## Priority A — required before any Ready decision for Draft PR #2

| ID | Question or missing evidence | Status | Required next evidence |
|---|---|---|---|
| SWS-OQ-018 | Is the bounded consolidation free of stale active status, duplicate professional truth and classification drift? | Pilot | Complete exact diff review against the consolidation readiness checklist. |
| SWS-OQ-019 | Are historical public/private concerns correctly classified without exposing private paths, mappings, markers or sensitive data? | Pilot | Review `PUBLIC_PRIVATE_REMEDIATION_REGISTER.md` and verify each disposition. |
| SWS-OQ-020 | Has an independent reviewer traced the final child PR Exact Head, scope, authority links and public/private boundary? | Missing | Complete the independent trace-review checklist against the final Exact Head. |
| SWS-OQ-021 | Is the final Draft PR #2 body current after consolidation is merged into the working branch? | Missing | Re-read Draft PR #2 body and working-branch Head after any authorized child-PR merge. |
| SWS-OQ-022 | Are Project Instructions consistent across every active STAR Project? | Missing | Verify each Project against the approved bootstrap and routing boundary. |

## Priority B — active Pilot validation

| ID | Question or missing evidence | Status | Required next evidence |
|---|---|---|---|
| SWS-OQ-004 | Can Command Desk maintain the Portfolio Ledger reliably over repeated updates? | Pilot | Continue verified coordination-only updates and record failures or recovery evidence. |
| SWS-OQ-005 | Does a Dispatch provide enough context without duplicating professional history? | Pilot | Compare bounded Dispatches across SWS, SAIG and M001. |
| SWS-OQ-006 | Is Report Back concise and complete enough to update durable status? | Pilot | Compare actual Report Backs with verified source updates. |
| SWS-OQ-007 | What makes a Scope Current, Stale or Unverified? | Candidate | Continue file-level fingerprint and operational-cadence tests before fixing thresholds. |
| SWS-OQ-008 | Does one Command Desk remain sufficient? | Candidate | Record actual overload, routing failure or access conflict. |
| SWS-OQ-009 | Is the public architecture repository appropriate for each coordination record? | Pilot | Continue classification checks and retain sensitive detail in private sources. |
| SWS-OQ-011 | Can `continue M001` resolve the correct Scope and runtime package without user reconstruction? | Pilot | Repeat in controlled environments and record contamination, missing-context and transfer limits. |
| SWS-OQ-012 | What token and file budgets are safe for Chat, Work and Codex? | Candidate | Measure entrypoint, payload and evidence loads during pilots. |
| SWS-OQ-013 | Should Context Packages be manually maintained, generated or hybrid? | Candidate | Continue manual Pilot before proposing automation. |
| SWS-OQ-014 | Is the Pilot Alias Registry safe and sufficient for verified Scope resolution? | Pilot | Validate uniqueness, collision stop, deprecation and tombstone behavior. |
| SWS-OQ-015 | Are classification, audience, redaction and evidence-access fields sufficient across public and private Context Packages? | Pilot | Validate through professional private sources using safe summaries and authorized evidence. |
| SWS-OQ-016 | Which environments support direct mode transfer and context inheritance? | Candidate | Record actual platform behavior; use Handoff where unavailable. |
| SWS-OQ-017 | Should Closed work ever use a governed Reopened state? | Candidate | Observe Pilot needs; until decided, use a new Activity or Contract. |

## Completed or superseded Pilot-start questions

| ID | Status | Basis |
|---|---|---|
| SWS-OQ-001 | Superseded | STAR Command Center Project Instructions were verified; SWS-OQ-022 now covers cross-Project consistency. |
| SWS-OQ-002 | Superseded | The three Pilot workstreams have verified coordination status; ongoing truth remains in professional sources and the Portfolio Ledger. |
| SWS-OQ-003 | Superseded | Generic ownership fields are established; product- and program-specific owner gaps remain in their professional sources. |
| SWS-OQ-010 | Superseded | Context Package locations are governed by professional sources and the current Pilot model; broader runtime coverage remains under SWS-OQ-011 and SWS-OQ-013. |

## Confirmed matters not to reopen without new evidence

- Correct Project and professional conversation are stated proactively.
- Users are not asked to repeat decisions available in authoritative records.
- GitHub stores durable structured memory, not raw chat archives.
- Runtime loading is progressive and file-level incremental; whole-repository and full-history loading are not default.
- The Portfolio Ledger is coordination-only.
- Professional truth remains in owning professional sources.
- Public records use safe summaries and pointers; private mappings and sensitive details remain outside this repository.
- Alias resolution determines where to load context, not the professional status itself.
- Automatic context loading is Not started.
- Mode transfer and future AI capability integration remain Candidate.
- The baseline is not frozen.
- No Ready, Freeze, Merge, policy activation, Gate passage, Product Commitment or Delivery authorization is created by this register.

## Deferred broader work

- complete Activity and Work Model;
- automatic Context Package generation and synchronization;
- future Agent orchestration;
- final role-specific Workspace views;
- full Memory and Knowledge lifecycle beyond the current structured-memory baseline.
