# STAR Product Delivery — Knowledge Review Register

| Field | Value |
|---|---|
| **Type / scope** | Governance register — ownership and review of durable Product Delivery knowledge |
| **Version / status** | v0.1.0 — Active working register; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | Product Delivery maintainers |
| **Last reviewed** | 2026-07-12 |
| **Review trigger** | File added, owner change, confirmed-decision change, contradictory guidance, real-Mission finding or freeze proposal |
| **Authoritative working source** | This repository path in Draft PR #1; `main` only after approved merge |
| **Affects** | Product Delivery Markdown, AI context assembly and future Mission teams |
| **Supersession** | None |
| **Access** | Public |

## Purpose

This register prevents important Markdown from becoming silently stale or unowned. It records the minimum review responsibility without forcing every short note to carry heavy governance metadata.

## Review states

- **Current:** reviewed against the current Decision Log and known evidence.
- **Review due:** a trigger occurred or the agreed interval passed.
- **Blocked:** correctness depends on missing authoritative information.
- **Superseded / archived:** no longer active; replacement or retention reason must be linked.

## High-impact knowledge register

| File / group | Accountable owner | Maintainer | Current status | Review trigger | Next review condition |
|---|---|---|---|---|---|
| `00_PROJECT_CHARTER.md` | STAR leadership | Product Delivery maintainers | Current working baseline | Strategy/scope change, real-Mission evidence or freeze proposal | Before any material scope or naming decision |
| `01_DECISION_LOG.md` | STAR leadership | Product Delivery maintainers | Current | New decision, supersession or detected conflict | Every material decision batch |
| `02_OPEN_QUESTIONS.md` | STAR leadership | Product Delivery maintainers | Current | Evidence added, question resolved or priority changes | After each validation batch |
| `03_RESEARCH_CANON.md` | STAR leadership | Architecture / Product Delivery maintainers | Current candidate | Source changes materially or a method is adopted/rejected | Before a Canon item becomes a frozen dependency |
| `05_ASSUMPTIONS.md` | STAR leadership | Product Delivery maintainers | Current | Validation evidence supports or contradicts a hypothesis | After each relevant test |
| `07_WORKING_METHOD.md` | STAR leadership | Product Delivery maintainers | Current confirmed method | New work-discipline decision or recurring execution friction | Before freeze and after real-Mission use |
| `11_FOUNDATION_CANDIDATE.md` | STAR leadership | Product Delivery maintainers | Candidate; blocked from freeze | Real-Mission evidence, role test or conflicting decision | After V1/V2 evidence becomes available |
| `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md` | STAR leadership | Architecture / Product Delivery maintainers | Candidate | Actual source/tool map, owner change, incident/audit finding | During V6 authoritative-source mapping |
| `14_AI_WORK_GOVERNANCE.md` | STAR leadership | AI governance / Product Delivery maintainers | Candidate | AI work test, risk/authority change or security/privacy finding | After code/test and A3 dry-run evidence |
| `15_VALIDATION_PLAN.md` | STAR leadership | Product Delivery maintainers | Candidate execution plan | New evidence, blocker change or freeze-gate change | After every completed validation step |
| `17_WORK_STATUS.md` | STAR leadership | Product Delivery maintainers | Active | Material task, blocker, decision or PR-state change | During every active work batch |
| `README.md`, `MANIFEST.md`, `CHANGELOG.md`, `GITHUB_SYNC_STATUS.md` | STAR leadership | Repository maintainers | Active repository controls | File set, release, branch or PR-state change | At the end of each repository batch |

## Ownership rule

- Governance groups may maintain repository-wide knowledge during this working phase.
- Before a document is frozen or used as a formal organizational standard, a named accountable human or formally approved governance body must be recorded.
- A file whose owner is unknown must be marked **Blocked**, downgraded to Candidate, or archived; it must not remain silently authoritative.

## Review evidence

A review is complete only when the reviewer checks:

1. consistency with `01_DECISION_LOG.md`;
2. open conflicts or assumptions;
3. current source links and version/state;
4. affected customers, teams, Missions and AI context;
5. whether the file should remain Candidate, become Confirmed/Frozen, or be superseded/archived.

Git history shows what changed. This register shows who is responsible for deciding whether the current content is still correct.

## Current finding

The highest-impact files now have either embedded metadata or an explicit entry in this register. Named individual owners, real-Mission ownership and the actual enterprise source/tool map remain unresolved and must not be invented.
