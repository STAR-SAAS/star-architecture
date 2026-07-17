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
required_files:
  - CONTEXT_PACKAGE.md
  - ACTIVE_DECISIONS.md
  - WORK_STATUS.md
optional_files:
  - OPEN_QUESTIONS.md
  - HANDOFF.md
  - <active brief / policy / architecture>
evidence_triggers:
  - changed branch or commit
  - decision conflict or supersession
  - material approval or risk claim
  - implementation or validation claim
```

## Runtime summary

- Objective:
- Current lifecycle state:
- Accountable owner:
- Current task:
- Next action:
- Blocker:
- Leadership decision required:

## Scope aliases

- Primary alias:
- Additional aliases:

## Active authority

- Global rules:
- Domain / Mission active decisions:
- Work Status:
- Latest Handoff:

## Loading instructions

1. Load required files only.
2. Compare live branch and commit with `last_verified_commit`.
3. Load optional files only when the current task or status points to them.
4. Load evidence only for a specific disputed, risky, approval-sensitive or implementation claim.
5. Never load the entire repository or full Decision Log by default.
6. Update verification metadata after a material verified change.

## Synchronization boundary

Synchronize material decisions, current status, approved artifacts and validation evidence. Exclude conversational noise, raw chat archives, secrets and protected data.
