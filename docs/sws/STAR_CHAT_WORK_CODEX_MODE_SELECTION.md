# STAR Chat / Work / Codex Mode Selection

| Mode | Primary use | Default context budget | Required freshness behavior | Escalate or switch when |
|---|---|---|---|---|
| Chat | clarification, decisions, concise status, lightweight drafting | smallest: entrypoint + active decisions + current Work Status | verify only operational facts used; compare required-file fingerprints where relevant | sustained research, multi-file artifacts or repository implementation begins |
| Work | research, analysis, document design, cross-source synthesis and professional review | medium: required payload plus selected optional files | verify source metadata and changed required-file blobs; load evidence progressively | code, tests, CI or repeated repository writes dominate |
| Codex | code, repository files, tests, CI, structured GitHub execution | task-specific: required payload + relevant tree/diff/tests | check branch, commit, required-file fingerprints, PR and CI before claiming current implementation | product, governance or leadership decision is Missing |

## Selection principles

1. Recommend or use the most suitable **available** mode according to dominant work.
2. A brief mismatch warning is enough when work can continue safely.
3. Mode does not grant authority; named humans and authoritative records remain controlling.
4. Direct mode switching and seamless context inheritance are Candidate and environment-dependent.
5. Where direct transfer is unavailable, preserve the existing Contract and create a Handoff.
6. Never require the user to repeat authoritative context merely because the mode changes.
7. Do not load the whole repository or full Decision Log by default.

## Token tiers

- **Tier 0:** Scope ID, classification, branch, commit, required-file versions, objective, next action and blocker.
- **Tier 1:** `CONTEXT_PACKAGE.md` entrypoint plus `ACTIVE_DECISIONS.md` and `WORK_STATUS.md` payload.
- **Tier 2:** Open Questions, brief, policy, architecture or latest Handoff when triggered.
- **Tier 3:** specific PR, issue, diff, test, research or Decision Log section.

Start at the lowest tier that can safely answer or execute.

## Freshness strategy

- Branch unchanged: reuse the verified runtime package.
- Branch changed but required-file blobs unchanged: package may remain Current.
- Required-file blob changed: reload only that file.
- Optional/evidence changes load only on trigger.
- Context metadata-only changes do not trigger full reload.
- Modification time alone is not proof of content freshness.
- Unavailable live state is Unverified; aged required operational content is Stale.

## Examples

- `continue M001`: conceptually resolves the M001 package and recommends Work or Codex from the next action; operational behavior remains Unverified until pilot evidence exists.
- `summarize SAIG status`: Chat loads the private SAIG entrypoint and Work Status; sensitive evidence loads only when authorized and necessary.
- `update the Command Desk ledger`: Chat verifies report-back sources; an available GitHub/Codex workflow performs repository writes. If transfer is unavailable, create a Handoff.
