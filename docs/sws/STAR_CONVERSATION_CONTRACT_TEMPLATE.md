# STAR Conversation Contract Template

> Create once at conversation start. Reuse on normal resume. Refresh metadata or `WORK_STATUS.md` when sufficient. Create a new Contract only when Scope, owner, authority or completion boundary changes materially.

| Field | Value |
|---|---|
| Project |  |
| Conversation |  |
| Professional scope / Activity ID |  |
| Accountable owner |  |
| Primary lifecycle state | Intake / Routed / Bootstrapped / Active / Review / Closed |
| Interrupt state | None / Waiting / Blocked |
| Prior state before interrupt |  |
| Preferred available mode | Chat / Work / Codex |
| Mode availability | Available / Candidate / Unavailable |
| Authoritative repositories / systems |  |
| Context package |  |
| Classification | Public / Internal / Confidential / Restricted |
| Permitted audience |  |
| Last verified branch / commit / timestamp |  |

## Objective

- Problem and desired outcome:
- Value receiver:
- In scope:
- Out of scope:

## Routing Gate

- Correct Project:
- Correct professional conversation:
- Correct available mode:
- Orchestration or professional execution:
- Outcome: Proceed / Proceed with brief warning / Route / Pause

## Runtime context manifest

### Entrypoint

- `CONTEXT_PACKAGE.md`

### Required payload

- `ACTIVE_DECISIONS.md`
- `WORK_STATUS.md`

### Optional files

- Open Questions / Missing Evidence
- active Mission or project brief
- policy / standard / architecture record
- latest Handoff
- referenced evidence or pull request

## Execution contract

- Expected artifacts or result:
- Batch plan:
- User interruption rule:
- Leadership escalation conditions:
- Durable records to update:
- Completion / handoff condition:

## Resume and lifecycle rule

- Normal resume reuses this Contract.
- Refresh only verification metadata or Work Status when the Contract remains valid.
- Waiting returns to the recorded prior state when awaited input arrives.
- Blocked returns to the recorded prior state when the blocker is resolved.
- Transfer requires a Handoff; the receiver begins at Bootstrapped and the sender records Transferred outside the active primary path.
- Closed is not silently reopened. New work uses a new Activity / Contract unless a future governed Reopened rule is approved.

## Data boundary

- Public summary allowed:
- Private authoritative source:
- Sensitive fields redacted:
- Evidence access boundary:
- Retention or review owner:

Public records contain only safe summaries and pointers. Employee permissions, customer or merchant facts, KYC/AML, payment data, incidents, commercial risk, credentials and private conversation content remain in approved private sources.

## State discipline

- Confirmed:
- Candidate:
- Missing:
- Unverified / Stale:

## Final check

- [ ] Existing Contract reused unless a material Contract field changed.
- [ ] Authoritative sources loaded, not reconstructed from chat memory.
- [ ] Required-file fingerprints checked where relevant.
- [ ] Mode recommendation reflects available tooling and dominant work.
- [ ] A Handoff exists when direct mode or conversation transfer is unavailable.
- [ ] Material decisions and status will be synchronized to GitHub.
- [ ] Sensitive data and conversational noise will not be copied.
- [ ] STAR Self-Review Gate will run after each material task.
