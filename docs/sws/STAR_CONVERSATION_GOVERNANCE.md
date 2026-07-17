# STAR Conversation Governance

| Field | Value |
|---|---|
| Document ID | SWS-CG-001 |
| Version / status | v0.1.0 — Working baseline; not frozen |
| Owner | STAR leadership |
| Maintainer | STAR Architecture maintainers |
| Scope | All STAR conversations, Projects and supported AI modes |
| Decision references | GWR-01–12; SWS-DEC-005–013 |

## 1. Purpose

STAR conversations are scoped execution spaces, not authoritative memory stores. This baseline defines how conversations are routed, resumed, transferred and closed without requiring the user to reconstruct prior context.

## 2. Scope and ownership

Every material conversation declares:

- Project and professional conversation;
- Scope ID, objective and value receiver;
- accountable human owner;
- authoritative repositories or systems;
- preferred Chat, Work or Codex mode;
- lifecycle state;
- escalation and completion boundaries.

The initiating AI or human owns the Bootstrap check. The conversation owner maintains scope clarity, Work Status and handoff quality. Business, product, governance, technical, risk and approval authority remains with named humans.

Cross-scope work is routed rather than silently absorbed.

## 3. Conversation Contract

At conversation start, material resume or scope change, establish the Contract in `STAR_CONVERSATION_CONTRACT_TEMPLATE.md`.

The Contract records destination, objective, boundaries, sources, runtime manifest, mode, escalation conditions, durable records and completion condition. It should remain concise and should link rather than duplicate authoritative detail.

## 4. Routing Gate

Before material execution, determine:

1. Is this the correct Project?
2. Is this the correct professional conversation?
3. Is the current mode suitable?
4. Is the request orchestration or professional execution?
5. Which Scope owns the authoritative result?
6. Is a material leadership decision required?

Outcomes:

- **Proceed** — Scope, conversation and mode match.
- **Proceed with brief warning** — work is safe but the mode is suboptimal.
- **Route** — another Project or conversation owns the work.
- **Pause** — authority, evidence or a material leadership decision blocks execution.

Warnings must be brief and should not interrupt reversible work unnecessarily.

## 5. Bootstrap and resume

Use progressive disclosure:

```text
Global → Domain → Product / Mission → Task → Evidence
```

The default runtime sequence is:

1. resolve the Scope or alias;
2. load its `CONTEXT_PACKAGE.md`;
3. verify repository, branch, commit and last-verified metadata;
4. load `ACTIVE_DECISIONS.md` and concise `WORK_STATUS.md`;
5. load optional Open Questions, Handoff, brief, policy or architecture only when triggered;
6. load specific evidence only for the active claim or task.

Do not load the whole repository, full chat history or full Decision Log by default. Do not ask the user to repeat decisions available in authoritative records.

A resume message should state only:

```text
Context loaded: <Scope and sources>
Objective: <current outcome>
Plan: <batched actions>
Blocker: <none or exact blocker>
User decision: <none or exact decision>
```

Long manual bootstrap prompts are fallback mechanisms, not the normal operating model.

## 6. Short-instruction resume

A short instruction such as `continue M001` should:

1. resolve `M001` through the authoritative Scope index;
2. identify Mission-001, its Project, professional conversation and repository;
3. load the required runtime package;
4. compare live and recorded branch/commit metadata;
5. state the current objective, next action, blocker and decision need;
6. choose Work or Codex according to the next action;
7. continue without asking the user to reconstruct confirmed requirements.

If the alias or package cannot be resolved, search authoritative indexes first. Ask the user only after authoritative resolution fails.

## 7. Chat / Work / Codex selection

Use `STAR_CHAT_WORK_CODEX_MODE_SELECTION.md`.

- **Chat:** clarification, decisions, concise status and lightweight drafting.
- **Work:** research, analysis, document design and cross-source synthesis.
- **Codex:** code, repository files, tests, CI and structured GitHub execution.

Mode is selected by dominant work. A mode label does not grant authority or change the source of truth.

## 8. Lifecycle and status

Canonical lifecycle:

```text
Intake → Routed → Bootstrapped → Active → Review → Waiting / Blocked → Transferred / Closed
```

Allowed durable statuses:

- Intake
- Routed
- Bootstrapped
- Active
- Review
- Waiting
- Blocked
- Transferred
- Closed

A conversation is Closed only when the requested outcome is complete, material records are synchronized, remaining work is explicitly transferred or recorded, and the STAR Self-Review Gate passes.

## 9. Decision and memory rules

- GitHub stores durable structured memory, not raw chat archives.
- Material Confirmed decisions enter the append-only `DECISION_LOG.md`.
- `ACTIVE_DECISIONS.md` is the concise runtime projection of currently effective decisions.
- `WORK_STATUS.md` is the primary task-resume record and must not become a chronological diary.
- Handoff records preserve unfinished state across conversation, owner or tool changes.
- Candidate, Confirmed, Frozen, Superseded, Missing, Stale and Unverified remain distinct.
- New decisions may not silently override active Decision IDs.
- Sensitive information remains in approved private systems.

Synchronize material decisions, current status, approved artifacts, validation evidence and authoritative links. Exclude conversational noise, repetitions, abandoned drafts, secrets and protected data.

## 10. Incremental loading and freshness

Each Context Package records:

- Scope ID and aliases;
- repository and branch;
- last verified commit and timestamp;
- required and optional file manifests;
- evidence-loading triggers;
- current freshness state.

If the live branch and commit match, reuse the required runtime set. If they changed, load changed required files first and only the affected optional records. Operational facts that cannot be verified are Stale or Unverified, never silently Current.

Final freshness thresholds remain Candidate until pilot evidence establishes suitable cadence by Scope.

## 11. Handoff and closure

Create or update a Handoff when:

- work changes Project, conversation, owner or AI tool;
- a material pause leaves unfinished work;
- context is likely to expire;
- another team or conversation must continue;
- closure leaves follow-up elsewhere.

The receiving conversation must be able to continue from concise state and links without asking the user to reconstruct history.

This baseline does not create, migrate or delete existing conversations.

## 12. User interruption and escalation

Continue in batches without repeated approval when work is reversible and inside confirmed scope.

Pause only when a decision:

- changes strategy, scope or governance authority;
- changes or supersedes an active Decision ID;
- creates material customer, security, compliance, financial or operational risk;
- commits costly or difficult-to-reverse architecture;
- authorizes rollout, production, migration, deletion or external commitment;
- requires leadership preference between valid alternatives.

When interrupted, preserve the prior current task and next action, then determine whether the new request belongs to the same Scope, should be queued, or should be routed.

## 13. Failure handling

### Missing

Record the missing fact, owner, impact and evidence required. Do not invent it.

### Stale

Verify the live source before acting. If unavailable, retain the last known value with its date and a Stale marker.

### Unverified or unavailable source

Use secondary evidence only as Unverified. Do not claim current state, approval or completion.

### Conflicting records

Apply Scope hierarchy, authority, Decision IDs and provenance. Escalate only if the conflict cannot be resolved through those rules.

### Tool failure

Preserve the last verified state, report the failed action precisely, avoid duplicate writes and provide a safe manual path.

## 14. Validation examples

### STAR AI Governance

- Command Desk routes governance work to `⭐ STAR AI Governance`.
- Runtime loads the private SAIG Context Package, active decisions and Work Status.
- Sensitive permission and employee evidence remains private.
- Full PR or Issue history loads only when validating a specific claim.
- Policy effectiveness, Wave A activation and pilot launch remain separate decisions.

### Mission-001 SmartQuote Foundation

- `continue M001` resolves Mission-001 and loads confirmed requirements and current Work Status.
- Requirements such as multiple Opportunities, Quote versioning, frozen cost/rule snapshots, configurable Rule Center and API-first design are not re-asked.
- Work handles blueprint and analysis; Codex handles implementation and tests.
- Material requirement changes pause for product leadership.

### STAR Command Desk

- Command Desk loads the portfolio coordination Context Package and ledger.
- It links professional sources rather than importing their detail.
- It verifies report-backs before updating status.
- It does not perform SAIG, SmartQuote or SAF professional execution.

## 15. Pilot usage

Pilot only in:

1. SWS-001 / SAF;
2. STAR AI Governance;
3. Mission-001 SmartQuote Foundation;
4. STAR Command Desk as the orchestration surface.

Measure routing accuracy, short-instruction resume success, files/tokens loaded, stale-state detection, repeated context requests, synchronization omissions, mode warnings, handoff quality and closure accuracy.

Do not freeze or broadly roll out the model until pilot evidence demonstrates usability and safe authority boundaries.

## 16. Enforcement

- Run the STAR Self-Review Gate after every material task or artifact.
- Update Decision Log, Active Decisions, Work Status, Open Questions, Context Package, Handoff and indexes as applicable.
- Do not rely on chat memory alone.
- Do not increase context loading merely because more repository content is available.
