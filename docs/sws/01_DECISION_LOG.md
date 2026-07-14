# SWS-001 · Decision Log

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Active confirmed working decisions; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-14 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2, branch `agent/star-os-global-working-rules` |
| **Scope** | SWS-001 · STAR Workspace Specification |

## Log rules

- Entries are append-only.
- Corrections use a new Decision ID and explicitly supersede the prior decision.
- Confirmed working decisions are not automatically approved or frozen standards.
- Tool-specific implementation details remain candidates until verified in actual use.

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

## Not decided or frozen

The following remain open:

- final SWS-001 v1.0 structure and freeze criteria;
- full Activity and Work Model;
- complete Memory and Knowledge architecture;
- automated synchronization between professional sources and portfolio ledger;
- validated freshness thresholds;
- final access model for sensitive portfolio information;
- whether future portfolio scale requires another management surface.
