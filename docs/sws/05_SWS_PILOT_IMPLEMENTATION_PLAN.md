# SWS-001 · Pilot Implementation Plan

| Field | Value |
|---|---|
| Document ID | SWS-PILOT-001 |
| Version / status | v0.1.0 — Working plan; not frozen |
| Owner | STAR leadership |
| Maintainer | STAR Architecture maintainers |
| Base | Draft PR #2 working branch at `71329151126ca358c04ac2689a9e406a8953bdd6` |
| Scope | SWS-001 pilot across SAIG, M001 and STAR Command Desk |

## 1. Objective

Convert the approved Conversation Governance baseline into a controlled, evidence-producing pilot without merging Draft PR #2 into `main`, freezing SWS-001, creating or migrating conversations, or activating automatic Context Package synchronization.

## 2. Pilot packages

### Package A — SAIG Context Package

Professional destination: `⭐ STAR AI Governance`.

Deliverables:

- private `CONTEXT_PACKAGE.md`;
- concise `ACTIVE_DECISIONS.md` projection;
- current `WORK_STATUS.md`;
- classification and access review;
- verification record for private-source loading;
- Report Back to Command Desk.

Required validation:

- no employee permissions, incident details or protected evidence copied into public architecture records;
- SAIG retains privacy, retention, employee-data, audit and AI-record authority;
- required-file fingerprints are recorded;
- policy effectiveness, Wave activation and pilot authorization remain separate states.

### Package B — M001 Context Package and resume test

Professional destination: `🚀 Mission-001 · SmartQuote Foundation`.

Deliverables:

- M001 `CONTEXT_PACKAGE.md`;
- `ACTIVE_DECISIONS.md` with confirmed product requirements;
- concise `WORK_STATUS.md`;
- authoritative alias registration for `M001` during the pilot;
- controlled `continue M001` resume test;
- files/tokens loaded and repeated-context requests recorded;
- Report Back to Command Desk.

Required validation:

- correct Project, professional conversation and repository resolve without user reconstruction;
- confirmed requirements are not re-asked;
- branch and required-file fingerprints are verified;
- optional evidence loads only on trigger;
- result remains Unverified until the controlled test completes.

### Package C — Command Desk Context Package and safe ledger update

Professional destination: `⭐ STAR Command Desk`.

Deliverables:

- coordination-only `CONTEXT_PACKAGE.md`;
- active coordination decisions and concise Work Status;
- safe public-summary classification review;
- verified Report Back ingestion procedure;
- safe Portfolio Ledger update method that avoids known truncation-prone whole-file writes;
- one complete Dispatch → Execute → Report Back → Verify → Update Status → Feedback cycle.

Required validation:

- Command Desk does not perform SAIG, M001 or SAF professional execution;
- professional detail remains linked, not imported;
- Stale, Missing and Unverified states are preserved;
- public ledger contains no protected operational detail.

## 3. Common implementation rules

Each package must:

1. use `CONTEXT_PACKAGE.md` as the entrypoint only;
2. use `ACTIVE_DECISIONS.md` and `WORK_STATUS.md` as required payload;
3. record classification, repository visibility, audience, public-summary permission, private source, redaction, evidence boundary and review owner;
4. record branch head and required-file blob SHAs with verification timestamps;
5. avoid full-repository, full-history and raw-chat loading by default;
6. keep Candidate, Confirmed, Missing, Stale and Unverified distinct;
7. reuse the existing Conversation Contract on normal resume;
8. create a Handoff when direct conversation or mode transfer is unavailable;
9. run STAR Self-Review Gate before Report Back;
10. not activate automatic generation or synchronization.

## 4. Pilot sequence

1. SAF approves this implementation plan and dispatch package structure.
2. Command Desk dispatches Package A, B and C to their professional destinations.
3. Each professional conversation implements and reviews its own package in its authoritative repository or approved private system.
4. Each destination returns a source-linked Report Back.
5. Command Desk verifies Report Backs and updates coordination status safely.
6. SAF performs cross-pilot assessment and records findings.
7. Leadership decides whether Draft PR #2 may progress toward final review; no automatic merge follows.

Packages A and B may execute in parallel after dispatch. Package C may prepare its Context Package in parallel, but its verified ledger cycle depends on at least one professional Report Back.

## 5. Evidence and metrics

Record for every package:

- exact repository, branch and commit;
- required-file blob SHAs;
- files loaded before useful work;
- estimated or measured token footprint where available;
- number of user context-reconstruction requests;
- alias-resolution result;
- stale-state detections;
- optional/evidence loads and triggers;
- classification or redaction findings;
- mode-transfer or Handoff result;
- Self-Review result;
- final state: Passed / Passed with findings / Failed / Unverified.

Numeric token and time thresholds remain Candidate. The pilot gathers evidence; it does not invent universal thresholds in advance.

## 6. Completion criteria

The pilot is complete only when:

- all three Context Packages exist in approved locations;
- the M001 controlled resume test has evidence;
- one verified end-to-end Command Desk cycle is complete;
- public/private boundary tests pass or remediation is recorded;
- required-file fingerprint behavior is demonstrated;
- token/file footprint is recorded for all three packages;
- remaining findings are classified and assigned;
- SAF performs a final cross-pilot review.

Completion of this pilot does not itself freeze SWS-001 or authorize merging Draft PR #2.

## 7. Stop conditions

Pause the affected package if:

- protected data would enter a public repository;
- the authoritative source or accountable owner is Missing;
- a Decision ID conflict cannot be resolved by provenance;
- a required-file fingerprint cannot be verified;
- implementation would require automatic synchronization, conversation migration or production rollout;
- a material leadership decision is required.

## 8. Current limitations

- canonical Alias Registry location remains open;
- Context Package canonical paths may differ by repository during the pilot;
- direct mode transfer is environment-dependent;
- automatic package generation is not authorized;
- Command Center Portfolio Ledger remains Stale / update pending until a safe verified update cycle completes.