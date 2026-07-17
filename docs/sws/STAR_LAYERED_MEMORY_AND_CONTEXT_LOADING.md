# STAR Layered Memory and Context Loading

| Field | Value |
|---|---|
| Document ID | SWS-MEM-001 |
| Version / status | v0.1.0 — Working baseline; not frozen |
| Scope | STAR organizational memory and runtime context loading |

## 1. Principle

GitHub is STAR's durable structured organizational memory for material decisions, status, approved artifacts and traceable evidence. It is not a raw chat archive.

Synchronize:

- material Confirmed decisions and supersession;
- current Work Status, next action, blocker and ownership;
- approved or reviewable artifacts;
- material validation evidence and authoritative links;
- handoffs required to resume or transfer work.

Exclude:

- conversational noise, repetitions and abandoned drafts;
- full AI transcripts unless explicitly required and approved;
- secrets, credentials, payment, KYC, customer, employee or other protected data;
- speculative claims presented without state labels.

## 2. Scope-level runtime package

Each active domain, product, Mission or material workstream should converge on:

```text
CONTEXT_PACKAGE.md
ACTIVE_DECISIONS.md
WORK_STATUS.md
DECISION_LOG.md
OPEN_QUESTIONS.md                 # when needed
HANDOFF.md                        # when active transfer/resume requires it
```

`CONTEXT_PACKAGE.md` is the default runtime entry point. It contains pointers and metadata, not duplicated full history.

## 3. Required and optional manifests

A context package declares:

```yaml
scope_id: M001
repository: STAR-SAAS/<repo>
branch: main
last_verified_commit: <sha>
last_verified_at: <timestamp timezone>
required_files:
  - CONTEXT_PACKAGE.md
  - ACTIVE_DECISIONS.md
  - WORK_STATUS.md
optional_files:
  - OPEN_QUESTIONS.md
  - HANDOFF.md
  - <active brief or policy>
evidence_triggers:
  - decision conflict
  - changed branch or commit
  - material risk or approval claim
  - implementation verification
```

Required files load by default. Optional files load only when the current task, state or conflict requires them.

## 4. Active decisions and history

- `ACTIVE_DECISIONS.md` is a compact runtime projection of all currently effective decisions for the Scope.
- `DECISION_LOG.md` remains the append-only historical authority, including Superseded decisions and provenance.
- Every active entry links to its Decision ID in the historical log.
- A runtime agent loads the full historical log only for conflict, audit, supersession or provenance review.

## 5. Work Status as resume authority

`WORK_STATUS.md` is the primary resume record and should remain concise:

- objective and boundary;
- lifecycle status;
- verified completed work;
- current task and next three actions;
- blockers and dependencies;
- leadership decision required;
- authoritative branch, commit and last-verified metadata;
- latest Handoff link when applicable.

It must not become a chronological diary.

## 6. Progressive disclosure

Load in this order:

```text
Global → Domain → Product / Mission → Task → Evidence
```

At each layer, load only the context package, active decisions and Work Status required to interpret the narrower layer. Evidence loads last and only for the active claim or action.

No default whole-repository, all-file, all-chat or full-history loading is permitted.

## 7. Incremental loading

1. Resolve the Scope alias, such as `M001`.
2. Read its `CONTEXT_PACKAGE.md`.
3. Compare recorded branch, commit and `last_verified_at` with the live source.
4. If unchanged, load the required runtime set only.
5. If changed, identify changed required files first.
6. Load optional files only when referenced by the current Work Status or task.
7. Load specific evidence for disputed, risky, approval-sensitive or implementation claims.
8. Update verification metadata after a successful material review.

## 8. Token budget

Token allocation is proportional to risk and work mode:

- Chat: target the required runtime set and one evidence item at a time.
- Work: required set plus selected optional files and bounded cross-source evidence.
- Codex: required set plus task-relevant repository tree, diff, tests and CI state.

When the budget is constrained, preserve in order:

1. scope and authority;
2. active decisions;
3. current objective, next action and blockers;
4. safety, approval and data boundaries;
5. evidence links;
6. historical explanation.

## 9. Freshness

Every runtime package records branch, commit and last-verified timestamp.

- **Current:** live source matches the recorded commit or the required files were freshly verified.
- **Stale:** operational facts exceeded the Scope's review trigger or the branch/commit changed without review.
- **Unverified:** live source could not be accessed or secondary evidence was used.
- **Missing:** a required record or owner does not exist.

Final freshness thresholds remain Candidate until pilot evidence shows appropriate cadence by Scope.

## 10. Short-instruction resume

For `continue M001`:

1. resolve `M001` to Mission-001 SmartQuote Foundation;
2. identify its Project, professional conversation and repository;
3. load the global runtime pointer and M001 `CONTEXT_PACKAGE.md`;
4. verify branch and commit;
5. load `ACTIVE_DECISIONS.md` and `WORK_STATUS.md`;
6. state objective, batched plan, blocker and decision need;
7. select Work or Codex from the next action;
8. continue without asking the user to repeat confirmed requirements.

If the alias is ambiguous or the package is Missing, search authoritative indexes first. Ask the user only after authoritative resolution fails.

## 11. Validation

### STAR AI Governance

The package points to the private SAIG repository and loads active governance decisions and current operational status. Sensitive permission evidence remains private; full PR/Issue history loads only when validating a specific state.

### Mission-001 SmartQuote Foundation

The package exposes confirmed requirements such as Opportunity multiplicity, Quote versioning, frozen pricing snapshots, configurable Rule Center and API-first design. Historical discussion is not loaded unless a requirement conflict arises.

### STAR Command Desk

The package loads the portfolio ledger rules and current ledger state. It links professional sources rather than importing their detail, preserving orchestration boundaries and a small runtime footprint.

## 12. Pilot measures

Track:

- successful short-instruction resumes;
- tokens or files loaded before useful work begins;
- repeated user-context requests;
- stale-state detection;
- unnecessary full-history loads;
- missed material synchronization;
- sensitive-data or authority-boundary failures.
