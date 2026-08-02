# STAR Context Package Template

```yaml
scope_id: <ID>
scope_name: <name>
project: <Project>
conversation: <professional conversation>
repository: <owner/repo>
branch: <branch>
last_verified_commit: <sha>
last_verified_at: <timestamp timezone>
freshness: Current | Stale | Unverified | Missing
classification: Public | Internal | Confidential | Restricted
repository_visibility: public | private
permitted_audience:
public_summary_allowed: true | false
private_authoritative_source:
sensitive_fields_redacted: true | false
evidence_access_boundary:
retention_or_review_owner:
context_generation: <integer or version>
entrypoint: CONTEXT_PACKAGE.md
required_files:
  - ACTIVE_DECISIONS.md
  - WORK_STATUS.md
required_file_versions:
  ACTIVE_DECISIONS.md:
    blob_sha: <sha>
    verified_at: <timestamp timezone>
  WORK_STATUS.md:
    blob_sha: <sha>
    verified_at: <timestamp timezone>
optional_files:
  - OPEN_QUESTIONS.md
  - HANDOFF.md
  - <active brief / policy / architecture>
evidence_triggers:
  - changed required-file blob
  - decision conflict or supersession
  - material approval or risk claim
  - implementation or validation claim
```

## Runtime summary

- Objective:
- Current primary lifecycle state:
- Interrupt state / prior state:
- Accountable owner:
- Current task:
- Next action:
- Blocker:
- Leadership decision required:

## Scope aliases

- Primary alias:
- Additional aliases:
- Alias registry reference:

## Active authority

- Global rules:
- Domain / Mission active decisions:
- Work Status:
- Latest Handoff:

## Loading instructions

1. Load this entrypoint once; do not recursively reload it as required payload.
2. Load `ACTIVE_DECISIONS.md` and `WORK_STATUS.md`.
3. Compare live branch head and required-file blob SHAs with recorded metadata.
4. Branch head unchanged: reuse the verified runtime package.
5. Branch head changed but required-file blobs unchanged: the runtime package may remain Current.
6. Required-file blob changed: load only that changed required file.
7. Optional or evidence-file changes load only when their trigger applies.
8. Context metadata changes alone do not trigger a full reload.
9. Never load the entire repository or full Decision Log by default.
10. Update file-level verification metadata only after successful verification.

## Public/private boundary

Public repositories may contain only safe summaries and pointers. Public Context Packages must not expose employee permissions, customer or merchant facts, KYC/AML, payment data, incidents, commercial risk, credentials or private conversation content. Private operational detail remains in approved private sources.

SAIG retains authority for AI privacy, retention, employee-data, audit and AI-record controls. SWS defines only the generic structure and routing boundary.

## Synchronization boundary

Synchronize material decisions, current status, approved artifacts and validation evidence. Exclude conversational noise, raw chat archives, secrets and protected data.
