# SWS-001 · Pilot Implementation Plan

| Field | Value |
|---|---|
| Document ID | SWS-PILOT-001 |
| Version / status | v0.2.0 — Revised working plan; ready for re-review; not frozen |
| Owner | STAR leadership |
| Maintainer | STAR Architecture maintainers |
| Base | Draft PR #2 working branch at `71329151126ca358c04ac2689a9e406a8953bdd6` |
| Scope | SWS-001 pilot across SAIG, M001 and STAR Command Desk |

## 1. Objective

Convert the approved Conversation Governance baseline into a controlled, evidence-producing pilot while preserving professional authority, explicit ownership, public/private data boundaries, recoverable failure paths and verifiable evidence.

## 2. Non-authorizations and non-goals

This plan does not authorize or cause any of the following:

- merging Draft PR #2 into `main`;
- freezing SWS-001;
- production deployment, formal rollout or organization-wide adoption;
- creating, migrating or deleting conversations;
- automatic Context Package generation or synchronization;
- Employee AI Use Policy effectiveness;
- Wave A activation;
- automatic authorization or activation of SAIG PILOT-001;
- transition of M001 into formal SmartQuote Delivery, implementation or production delivery;
- replacement of professional Projects, professional conversations, authoritative repositories or named accountable owners;
- transfer of professional execution responsibility to Command Desk.

Completion of this pilot is evidence for later review only. It does not itself authorize any item above.

## 3. Common ownership model

Every Package must record the following before it may enter Active:

```yaml
accountable_owner:
maintainer:
execution_owner:
professional_reviewer:
report_back_approver:
owner_status: Confirmed | Missing
```

Rules:

- `accountable_owner` must be a named person; `STAR leadership`, a department or a team name is not sufficient.
- If a name cannot be confirmed from an authoritative source, the field remains empty and `owner_status` remains `Missing`.
- A Package with `owner_status: Missing` must remain Waiting or Blocked and must not enter Active.
- Command Desk performs dispatch, verification and coordination only; it does not become the professional executor or reviewer by default.
- A person may hold multiple roles only when the overlap is explicit and permitted by the owning Scope.

## 4. Pilot packages

### 4.1 Package A — SAIG Context Package

Professional destination: `⭐ STAR AI Governance`.

Ownership at plan revision time:

```yaml
accountable_owner:
maintainer:
execution_owner:
professional_reviewer:
report_back_approver:
owner_status: Missing
```

The names remain Missing until confirmed from the authoritative SAIG source. Package A must not enter Active before resolution.

Deliverables:

- private `CONTEXT_PACKAGE.md`;
- concise `ACTIVE_DECISIONS.md` projection;
- current `WORK_STATUS.md`;
- classification, access and retention review;
- verification record for private-source loading;
- public-safe Report Back to Command Desk.

Before activation, Package A must confirm and record:

```yaml
private_context_location:
repository_or_system_visibility:
permitted_audience:
read_permission_boundary:
write_permission_boundary:
classification:
retention_owner:
review_owner:
private_source_access_verification:
```

SAIG retains authority for AI privacy, retention, employee-data, audit and AI-record controls. Policy effectiveness, Wave activation and Pilot authorization remain independent states and must not be inferred from Context Package completion.

#### Two-layer reference model

Public coordination records use:

```yaml
public_reference_id: <opaque-id>
```

Private professional records may use:

```yaml
private_authoritative_source: <private-only repository/path/issue/url>
```

Rules:

- public `star-architecture` records may contain only `public_reference_id` and public-safe summaries;
- the real repository, path, Issue, URL or system identifier exists only in the approved private professional source;
- public IDs, titles and summaries must not encode employee, customer, merchant, Incident, investigation, risk or internal-control semantics;
- a mapping between public and private references must remain in an access-controlled private source;
- access to the private source must be verified before the Package is marked Passed.

Public-field allowlist:

- Portfolio Item ID;
- public-safe title;
- high-level status;
- priority;
- destination Project and conversation name when those names are approved for public use;
- accountable owner only when publication is approved;
- current focus and next action written as safe summaries;
- blocker category without protected detail;
- decision-needed indicator without protected detail;
- `public_reference_id`;
- last reported, last verified and freshness values;
- final result state.

Private-only fields:

- `private_authoritative_source` and actual repository/path/Issue/URL;
- employee permissions, identities not approved for publication and access-entitlement detail;
- customer and merchant identities or case detail;
- Incident, investigation, audit and control evidence;
- risk narratives, protected findings and remediation evidence;
- private Decision content and sensitive Work Status detail;
- raw prompts, chats, logs and operational evidence;
- access-control and retention implementation detail.

Required validation:

- no protected information is copied into public architecture or Ledger records;
- the opaque-reference mapping resolves only for permitted users;
- required-file fingerprints are recorded and verified;
- SAIG authority and activation states remain unchanged;
- repository or system visibility and read/write boundaries are verified.

### 4.2 Package B — M001 Context Package and resume test

Professional destination: `🚀 Mission-001 · SmartQuote Foundation`.

Ownership at plan revision time:

```yaml
accountable_owner:
maintainer:
execution_owner:
professional_reviewer:
report_back_approver:
owner_status: Missing
```

The names remain Missing until confirmed from the authoritative M001 source. Package B must not enter Active before resolution.

Deliverables:

- M001 `CONTEXT_PACKAGE.md`;
- `ACTIVE_DECISIONS.md` containing confirmed SmartQuote requirements;
- concise `WORK_STATUS.md`;
- Pilot Alias Registry entry for `M001`;
- controlled `continue M001` resume test;
- file-load, Token-footprint and repeated-context-request evidence;
- Report Back to Command Desk.

#### Pilot Alias Registry

The Pilot must record:

```yaml
registry_location:
registry_status: Pilot Candidate
alias_owner:
write_authority:
alias_uniqueness_rule: exact alias must map to exactly one active Scope
collision_handling: stop resolution; mark Blocked; require authoritative correction
migration_rule: preserve provenance and redirect only after approved verification
deprecated_alias_rule: retain tombstone and replacement pointer; do not silently reuse
pilot_exit_rule: leadership decides retain, migrate or deprecate before Pilot closure
```

Rules:

- the temporary Registry is a Pilot Candidate and is not the final canonical Registry;
- `M001` must resolve to exactly one active Mission Scope;
- Alias values must be read from the Registry, not inferred from chat history or AI memory;
- a collision or ambiguous mapping stops resolution and records Blocked;
- only the recorded `write_authority` may modify an Alias entry;
- every modification preserves the previous value, reason, actor and verification timestamp;
- Pilot closure requires an explicit decision to retain, migrate or deprecate the entry.

#### Controlled `continue M001` test script

1. Begin from a blank or deliberately minimal context that does not contain the M001 working history.
2. Record the environment, available tools, start time and initiating prompt.
3. Enter `continue M001`.
4. Resolve `M001` through the Pilot Alias Registry and record the exact result.
5. Verify the correct Project, professional conversation, repository, branch and commit.
6. Load the Context Package entrypoint.
7. Load required `ACTIVE_DECISIONS.md` and `WORK_STATUS.md` payloads.
8. Verify branch head and required-file blob SHAs before useful work.
9. Record entrypoint, required, optional and evidence file counts; optional and evidence files load only on a recorded trigger.
10. Verify confirmed SmartQuote requirements are available without asking the user to repeat them.
11. Produce the current objective, next action, blocker and decision-needed summary.
12. Recommend Chat, Work or Codex only from the current task and tools actually available in that environment.
13. Record any Alias failure, source mismatch, stale fingerprint, repeated-context request, unavailable tool or Handoff.
14. Run the STAR Self-Review Gate and assign the final result state.

Passing conditions:

- `M001` resolves uniquely and correctly;
- Project, professional conversation, repository, branch and commit are correct;
- confirmed SmartQuote requirements are not re-requested from the user;
- required-file fingerprints are successfully verified;
- full repository history, raw chat history and unrelated evidence are not loaded by default;
- the output accurately states the objective, next action, blocker and decision needed;
- mode recommendation is based on actual task and available tools;
- the result does not claim formal SmartQuote Delivery has begun.

#### M1 Gate

- Context Package Pilot completion does not authorize formal SmartQuote Delivery.
- M001 must not enter formal implementation or delivery before M1 is Passed and leadership commitment authorization is recorded.
- Any missing M1 evidence or authorization keeps formal delivery Blocked.

### 4.3 Package C — Command Desk Context Package and safe Ledger update

Professional destination: `⭐ STAR Command Desk` for coordination execution only; professional review of the protocol remains in SAF.

Ownership at plan revision time:

```yaml
accountable_owner:
maintainer:
execution_owner:
professional_reviewer:
report_back_approver:
owner_status: Missing
```

The names remain Missing until confirmed from the authoritative Command Center source. Package C must not enter Active before resolution.

Deliverables:

- coordination-only `CONTEXT_PACKAGE.md`;
- active coordination decisions and concise Work Status;
- safe public-summary classification review;
- verified Report Back ingestion procedure;
- executed Safe Ledger Update Protocol;
- one complete Dispatch → Execute → Report Back → Verify → Update Status → Feedback cycle.

Command Desk must not perform SAIG, M001 or SAF professional work. Its Context Package and Ledger contain portfolio-coordination information only; professional details remain in linked private or professional authoritative sources.

#### Safe Ledger Update Protocol

1. Read the current complete Ledger from its authoritative branch.
2. Record the current Ledger blob SHA and verified commit.
3. Identify exactly one target Portfolio Item and the fields authorized for update.
4. Generate the smallest expected semantic change and retain a pre-write copy for comparison.
5. Do not use a known truncation-prone or otherwise unverifiable whole-file replacement path.
6. Bind the write to the exact current blob SHA or equivalent optimistic-concurrency control.
7. If the SHA has changed, stop, mark Waiting or Blocked, re-read and re-evaluate; do not overwrite.
8. After the write, read the complete Ledger again.
9. Verify every intended target field.
10. Verify document length, headings, table structure, item count and all non-target regions.
11. Compare the before/after diff and confirm there are no unplanned changes.
12. If truncation or unexpected changes are detected, mark Failed and do not repeat the overwrite blindly.
13. Preserve the previous verified commit and blob SHA as the recovery point.
14. Restore or correct only through a separately verified operation using the recovery point.
15. Change Ledger freshness from Stale to Current only after all checks pass and the verification time is recorded.

Package C completion gate:

- its Context Package may be prepared in parallel;
- it may test read-only verification in parallel;
- it must not declare the end-to-end cycle Passed until at least one Package A or Package B professional Report Back has been independently verified and safely ingested;
- failure of Ledger integrity makes Package C Failed regardless of the professional Report Back result.

## 5. Common implementation rules

Each Package must:

1. use `CONTEXT_PACKAGE.md` as the entrypoint;
2. use `ACTIVE_DECISIONS.md` and `WORK_STATUS.md` as required payload;
3. record classification, visibility, audience, public-summary permission, redaction, evidence boundary, retention and review ownership;
4. record branch head and required-file blob SHAs with verification timestamps;
5. avoid full-repository, full-history and raw-chat loading by default;
6. keep Candidate, Confirmed, Missing, Stale, Failed and Unverified distinct;
7. reuse the existing Conversation Contract on normal resume;
8. create a Handoff when work continues across conversation, mode or accountable responsibility;
9. run the STAR Self-Review Gate before Report Back;
10. not activate automatic generation or synchronization;
11. preserve professional authority and named accountability;
12. stop before any non-authorized production or formal delivery transition.

## 6. Pilot sequence and dependencies

1. SAF reviews and approves the implementation plan and Package structure.
2. Named owners and required locations are resolved; Packages with Missing ownership remain Blocked.
3. Command Desk dispatches Package A, B and C to their approved destinations.
4. Each professional conversation implements and reviews its own Package in its authoritative repository or approved private system.
5. Each destination returns a source-linked, public-safe Report Back.
6. Command Desk verifies the Report Back and performs the Safe Ledger Update Protocol.
7. SAF performs the cross-Pilot assessment and records findings.
8. Leadership decides whether Draft PR #2 may progress toward final review; no automatic merge follows.

Package A and Package B may execute in parallel only after their owners, locations and authority boundaries are Confirmed. Package C may prepare in parallel, but its end-to-end validation depends on at least one verified professional Report Back.

## 7. Evidence and metrics

Record for every Package:

- exact repository or approved system, branch and commit where applicable;
- required-file blob SHAs;
- user context-reconstruction request count;
- Alias-resolution result where applicable;
- stale-state detections;
- optional and evidence loads with trigger reason;
- classification and redaction findings;
- mode-transfer or Handoff result;
- Self-Review result;
- final result state.

### 7.1 Token footprint

```yaml
token_footprint:
  status: Measured | Estimated | Unavailable
  value:
  unit:
  method:
  confidence:
```

Rules:

- `Measured` requires a direct tool or platform measurement and records the measurement method.
- `Estimated` records the estimator or method and an honest confidence level.
- character count, file size or subjective judgment must not be presented as an exact Token count.
- when a defensible value is unavailable, use `Unavailable` and leave `value` empty.
- numeric Token and time thresholds remain Candidate until Pilot evidence supports a later decision.

### 7.2 File loading boundary

Measurement start: receipt of the execution prompt.

Measurement end: the first executable plan or valid professional judgment produced from verified context.

Record:

```yaml
entrypoint_files:
required_payload_files:
optional_files:
evidence_files:
duplicate_loads:
```

A load repeated only because a fingerprint changed is not classified as an avoidable duplicate; the reason must be recorded.

## 8. Final result definitions

- **Passed:** all mandatory validations pass; no unresolved material risk remains.
- **Passed with findings:** the core objective is achieved; only non-blocking findings remain, and every finding has a named owner, remediation action and due date or review trigger.
- **Failed:** a data-boundary, authority, integrity or execution failure occurs, including Ledger corruption or an unauthorized transition.
- **Unverified:** authoritative evidence cannot be accessed or validated; success must not be inferred.

Rules:

- Failed and Unverified must not be recorded as complete or counted toward Pilot completion.
- Passed with findings is not permitted when any material risk, Missing owner or protected-data exposure remains.
- Final state must include supporting evidence and verification time.

## 9. Waiting, Blocked, Failed and Unverified recovery

Every affected path must record:

```yaml
current_status:
prior_state:
blocker:
failure_or_missing_evidence:
last_verified_commit:
last_verified_blob_sha:
recovery_owner:
next_recovery_action:
handoff_required: true | false
```

Rules:

- update the owning `WORK_STATUS.md` immediately after a material interruption;
- preserve the last verified state and evidence;
- do not blindly repeat a failed tool write;
- if work crosses conversation, mode or accountable responsibility, create a Handoff;
- after verified recovery, return to the recorded `prior_state` rather than inferring a new state;
- a missing material leadership decision keeps the Package Blocked;
- a Missing recovery owner keeps the Package Blocked;
- Failed or Unverified remains unresolved until a new verified result supersedes it with provenance.

## 10. Completion criteria

The Pilot is complete only when:

- all three ownership records are Confirmed with named accountable owners;
- all three Context Packages exist in approved locations;
- Package A public/private boundary and private-access tests pass;
- the M001 controlled resume test passes with evidence;
- the Pilot Alias Registry entry is resolved and its exit treatment is assigned;
- one verified end-to-end Command Desk cycle is Passed;
- the Safe Ledger Update Protocol is demonstrated without truncation or unintended change;
- required-file fingerprint behavior is demonstrated;
- Token and file-load footprint is recorded for all three Packages;
- all findings are classified and assigned;
- no Package remains Failed or Unverified;
- SAF completes a final cross-Pilot review.

Pilot completion does not freeze SWS-001, authorize Draft PR #2 merge, activate SAIG controls or authorize formal SmartQuote Delivery.

## 11. Stop conditions

Pause the affected Package if:

- protected data would enter a public repository or public Ledger;
- the authoritative source, named accountable owner or recovery owner is Missing;
- a Decision ID or Alias conflict cannot be resolved by provenance;
- a required-file fingerprint cannot be verified;
- Ledger integrity cannot be demonstrated;
- implementation would require automatic synchronization, conversation creation/migration/deletion, production rollout or formal delivery activation;
- M1 or leadership commitment authorization is missing for formal SmartQuote Delivery;
- a material leadership decision is required.

Apply the recovery record in Section 9 whenever a stop condition is reached.

## 12. Current Missing or Candidate items

- named accountable, maintenance, execution, review and Report Back approval roles for Packages A, B and C are Missing;
- Package A private Context Package location and access boundary are Missing;
- Pilot Alias Registry location, owner and write authority are Missing;
- the canonical long-term Alias Registry remains Candidate;
- direct mode transfer remains environment-dependent Candidate;
- numeric Token and time thresholds remain Candidate;
- automatic Context Package generation and synchronization remain unauthorized;
- Command Center Portfolio Ledger remains Stale until the Safe Ledger Update Protocol is successfully demonstrated;
- formal M001 M1 evidence and leadership commitment authorization remain separate from this Pilot.
