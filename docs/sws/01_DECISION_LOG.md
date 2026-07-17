# SWS-001 · Decision Log

| Field | Value |
|---|---|
| **Version / status** | v0.2.1 — Active confirmed working decisions; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 plus PR #3 proposed record version until approved merge |
| **Scope** | SWS-001 · STAR Workspace Specification |

## Authority note

- Decision basis may be leadership-confirmed before the corresponding record version is merged.
- Entries introduced or corrected in PR #3 are proposed record versions until PR #3 is merged into the Draft PR #2 branch.
- After that merge, they become part of the Draft PR #2 working baseline; they are still not frozen and do not enter `main` unless Draft PR #2 is separately merged.

## Log rules

- Entries are append-only.
- Corrections use a new Decision ID and explicitly preserve or supersede the prior decision.
- Confirmed working decisions are not automatically approved or frozen standards.
- Tool-specific implementation details remain Candidate until verified in actual use.

## Decisions

| ID | Decision | Status | Scope | Basis / note |
|---|---|---|---|---|
| **SWS-DEC-001** | STAR Workspace uses a scope-governed, record-backed and context-driven platform model. Context is a runtime derived view; authoritative records remain in declared source systems. | Confirmed working direction; not frozen | SWS-001 | Accepted during SWS architecture review |
| **SWS-DEC-002** | The minimum information model consists of Scope, Actor, Capability, Activity, Record and Context Package, with Typed Relationship as a structural primitive. Artifact is a Record subtype; Actor and Capability remain separate. | Confirmed working direction; not frozen | SWS-001 | Accepted during core-object review |
| **SWS-DEC-003** | Every non-global Scope has one governance parent; cross-scope relationships use typed links. Rules may propagate downward, but membership, access, capabilities, records and context do not automatically inherit. | Confirmed working direction; not frozen | SWS-001 | Accepted during Scope Model review |
| **SWS-DEC-004** | Authorization separates Actor, Principal, Scope-bound Role Assignment, provider-neutral Capability and conditional Grant. Material capability defaults to deny; AI execution retains named human accountability. | Confirmed working direction; not frozen | SWS-001 | Accepted during authorization review |
| **SWS-DEC-005** | Launch STAR Command Center as a separate Project with only `⭐ STAR Command Desk`; use it only for intake, prioritization, routing, portfolio status and feedback. Professional execution remains in professional Projects. | Confirmed launch direction; implementation incomplete | SWS-001 / STAR Command Center | Explicitly confirmed by the user; Project and Chat reported created |
| **SWS-DEC-006** | `docs/sws/command-center/STAR-PORTFOLIO-STATUS.md` in `STARSAAS/star-architecture` is the authoritative portfolio-coordination ledger during the pilot. It is not authoritative for professional detail. | Confirmed working implementation decision; not frozen | SWS-001 / STAR Command Center pilot | Established by the authority-source task on 2026-07-14 |
| **SWS-DEC-007** | The Command Center pilot covers only SWS-001, STAR AI Governance and Mission-001 SmartQuote Foundation. No existing conversations are migrated or deleted during the pilot. | Confirmed launch direction | STAR Command Center pilot | Explicitly confirmed by the user |
| **SWS-DEC-008** | The operating loop is Dispatch → Execute → Report Back → Verify → Update Status → Feedback. Cross-project status must not rely only on chat memory. | Confirmed launch direction | STAR Command Center pilot | Explicitly confirmed by the user |
| **SWS-DEC-009** | Weekly Planning, Monthly Review, Dashboard and other management conversations are not created until actual usage proves a concrete need. | Confirmed launch direction | STAR Command Center pilot | Explicitly confirmed by the user |
| **SWS-DEC-010** | Every material STAR conversation uses a scope and ownership Contract, Routing Gate, lifecycle state and durable handoff/closure rules; the correct Project, conversation and mode are stated proactively. | Leadership-confirmed basis; proposed record version in PR #3; not frozen | All STAR conversations | Confirmed user requirements in DSP-001-004 |
| **SWS-DEC-011** | Chat, Work and Codex are selected by dominant work type. A brief mismatch warning is required, but authority remains in declared records and named humans. | Leadership-confirmed basis; proposed record version in PR #3; not frozen | STAR conversation execution | Confirmed user requirements in DSP-001-004 |
| **SWS-DEC-012** | GitHub is durable structured organizational memory, not a raw chat archive. Material decisions, status and evidence synchronize to GitHub while noise and sensitive data are excluded. | Leadership-confirmed basis; proposed record version in PR #3; not frozen | STAR organizational memory | Additional confirmed requirement in DSP-001-004 |
| **SWS-DEC-013** | Scope-level `CONTEXT_PACKAGE.md`, `ACTIVE_DECISIONS.md` and concise `WORK_STATUS.md` form the default runtime set. Loading is incremental by branch, required-file version and freshness metadata; whole-repository and full-history loading are not default. | Leadership-confirmed basis; proposed record version in PR #3; not frozen | Runtime context loading | Additional confirmed requirement in DSP-001-004 |
| **SWS-DEC-014** | The repository containing the SWS-001 portfolio ledger was subsequently transferred from `STARSAAS/star-architecture` to `STAR-SAAS/star-architecture`. The portfolio-ledger governance intent of SWS-DEC-006 remains active; only the repository-location identity is corrected, and the original confirmed decision remains historically visible. | Leadership-confirmed repository-state correction; proposed record version in PR #3; not frozen | SWS-001 / STAR Command Center pilot | Repository transfer verified after SWS-DEC-006; does not silently rewrite SWS-DEC-006 |

## Not decided or frozen

- final SWS-001 v1.0 structure and freeze criteria;
- full Activity and Work Model;
- automated synchronization and generation of context packages;
- validated token and freshness thresholds by Scope and mode;
- final access model for sensitive portfolio information;
- exact canonical location and naming convention for context packages in every repository;
- authoritative Scope Alias Registry location and collision rules;
- whether future portfolio scale requires another management surface.
