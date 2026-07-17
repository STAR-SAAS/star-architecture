# STAR Chat / Work / Codex Mode Selection

| Mode | Primary use | Default context budget | Required freshness behavior | Escalate or switch when |
|---|---|---|---|---|
| Chat | clarification, decisions, concise status, lightweight drafting | smallest: context package + active decisions + current Work Status | verify only the operational facts used in the answer | sustained research, multi-file artifacts or repository implementation begins |
| Work | research, analysis, document design, cross-source synthesis and professional review | medium: required manifest plus selected optional files | verify source metadata and load evidence progressively | code, tests, CI or repeated repository writes dominate |
| Codex | code, repository files, tests, CI, structured GitHub execution | task-specific: context package + active decisions + Work Status + repository tree/diff/tests needed for the task | check branch, commit, PR and CI state before claiming current implementation | a product, governance or leadership decision is Missing |

## Selection principles

1. Select the mode by the dominant work, not by where the conversation happened to begin.
2. A brief mismatch warning is enough when work can continue safely.
3. Mode does not grant authority; named humans remain accountable.
4. Do not load the whole repository or full Decision Log by default.
5. Load evidence only when the active task or conflict requires it.
6. Switch modes without making the user repeat confirmed context; preserve the Contract and Handoff.

## Token-budget strategy

- **Tier 0 — Resume header:** scope ID, branch, commit, last verified time, objective, next action and blocker.
- **Tier 1 — Required runtime set:** `CONTEXT_PACKAGE.md`, `ACTIVE_DECISIONS.md`, `WORK_STATUS.md`.
- **Tier 2 — Conditional records:** Open Questions, active brief, policy, architecture or latest Handoff.
- **Tier 3 — Evidence:** specific PR, issue, diff, test, research or historical Decision Log sections.

Start at the lowest tier that can safely answer or execute. Expand only on trigger.

## Freshness strategy

- Compare the context package's recorded branch and commit with the live source.
- If unchanged, reuse the verified runtime set and avoid reloading history.
- If changed, load changed required files first, then only affected optional records.
- Mark unavailable live state as Unverified; mark an aged operational record as Stale.
- Do not treat a recent file modification timestamp alone as proof that all content is current.

## Examples

- `continue M001`: Work loads the M001 required runtime set; switches to Codex only when the next action is implementation.
- `summarize SAIG status`: Chat loads SAIG context package and Work Status; evidence is loaded only for disputed or recent facts.
- `update the Command Desk ledger`: Chat verifies linked professional reports; Codex/GitHub workflow performs the repository update.
