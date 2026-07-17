# STAR OS · Product Delivery — Working Memory Baseline

**Version:** v0.3.0  
**Date:** 2026-07-17 (Asia/Singapore)  
**Status:** Working baseline; not frozen  
**Purpose:** Preserve confirmed decisions and translate research into material that teams can understand and use.

## Current work

Read [`17_WORK_STATUS.md`](17_WORK_STATUS.md) for completed work, evidence gates, blockers and whether user input is required.

## Active authoritative Mission

- [`missions/M001/README.md`](missions/M001/README.md) — Mission-001 · SmartQuote Foundation record index.
- [`missions/M001/MISSION_BRIEF.md`](missions/M001/MISSION_BRIEF.md) — first authoritative Mission Brief.
- [`missions/M001/DECISION_LOG.md`](missions/M001/DECISION_LOG.md) — Mission-scoped confirmed decisions.
- [`missions/M001/WORK_STATUS.md`](missions/M001/WORK_STATUS.md) — current Mission state and next actions.
- [`missions/M001/WALKTHROUGH_PREPARATION.md`](missions/M001/WALKTHROUGH_PREPARATION.md) — M1 participant and evidence preparation.

M001 is `Candidate — Baseline Confirmed`. It is not Committed, formal implementation has not started and it has not been routed to SmartQuote Delivery.

## Start here

Most participants should read only one or two files:

1. [`11_FOUNDATION_CANDIDATE.md`](11_FOUNDATION_CANDIDATE.md) — one-page candidate model.
2. [`templates/MISSION_BRIEF.md`](templates/MISSION_BRIEF.md) — the team-facing Mission template.
3. For the real active Mission, read [`missions/M001/MISSION_BRIEF.md`](missions/M001/MISSION_BRIEF.md).
4. See the desk examples only when example formatting is useful:
   - [`examples/MISSION_SMARTQUOTE_MERCHANT_DISCOUNT_RULE.md`](examples/MISSION_SMARTQUOTE_MERCHANT_DISCOUNT_RULE.md)
   - [`examples/MISSION_GATEHUB_PSP_CONNECTOR.md`](examples/MISSION_GATEHUB_PSP_CONNECTOR.md)

The examples are illustrative only. They are not evidence that a real active Mission has passed validation.

## Read by responsibility

| Participant | Read first |
|---|---|
| Leadership / Sponsor | Work Status and Foundation candidate, then the active Mission Brief |
| Product / Project / Architecture | Active Mission Brief, Mission Decision Log and responsibility views |
| Engineering / QA / Operations | Active Mission Brief, Walkthrough Preparation and linked technical evidence |
| AI team / agents | Active Mission Brief, authorized context and AI governance |
| Security / Risk / Compliance / Legal / Finance | Mission risk/approval section and linked evidence |
| Repository maintainers | Decision Logs, Open Questions, Working Method, Work Status and Changelog |

Detailed research is not required reading for front-line contributors.

## Repository contents

| File | Purpose |
|---|---|
| `00_PROJECT_CHARTER.md` | Purpose, scope, constraints and success criteria |
| `01_DECISION_LOG.md` | Confirmed Product Delivery working agreements and decisions |
| `02_OPEN_QUESTIONS.md` | Unresolved questions that must not be presented as facts |
| `03_RESEARCH_CANON.md` | Reviewed external methods and current STAR posture |
| `04_SUPERSEDED_IDEAS.md` | Rejected or replaced ideas and reasons |
| `05_ASSUMPTIONS.md` | Hypotheses that still require validation |
| `06_STAKEHOLDER_MAP.md` | External and internal stakeholder coverage |
| `07_WORKING_METHOD.md` | How work is researched, decided, recorded and delivered |
| `08_PRODUCT_DELIVERY_DRAFT_AUDIT.md` | Audit of the three early Product Delivery drafts |
| `09_GLOSSARY.md` | Shared working terms |
| `10_MODEL_VALIDATION.md` | SmartQuote and GateHub desk validation |
| `11_FOUNDATION_CANDIDATE.md` | One-page candidate foundation and Mission definition |
| `12_RESPONSIBILITY_AND_ROLE_VIEWS.md` | Responsibility model and participant first views |
| `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md` | Authoritative-source map and knowledge lifecycle candidate |
| `14_AI_WORK_GOVERNANCE.md` | Candidate AI work levels, authority and validation boundaries |
| `15_VALIDATION_PLAN.md` | Evidence status and freeze requirements |
| `16_ACTIVE_MISSION_INTAKE.md` | Active Mission intake and evidence-gap state |
| `17_WORK_STATUS.md` | Current Product Delivery status, blockers and next actions |
| `18_DECISION_RECORD_VALIDATION.md` | Cross-domain test of the generic Decision Record |
| `19_AI_WORK_CONTROL_DRY_RUN.md` | A1/A2 AI governance dry run |
| `20_ROLE_VIEW_DESK_WALKTHROUGH.md` | Desk validation of participant first views |
| `21_AI_CONTEXT_PACKAGE_TEST.md` | A2 AI context-package validation |
| `22_KNOWLEDGE_METADATA_AUDIT.md` | Durable-knowledge metadata audit |
| `23_KNOWLEDGE_REVIEW_REGISTER.md` | Ownership and review register for high-impact knowledge |
| `24_AI_A3_HIGH_IMPACT_DRY_RUN.md` | Design-level A3 production/customer-impact dry run |
| `missions/M001/` | Authoritative Mission-001 SmartQuote Foundation record set |
| `templates/` | Mission, decision, intake, AI context and knowledge-metadata templates |
| `examples/` | SmartQuote/GateHub desk examples and Decision Record examples |
| `GITHUB_SYNC_STATUS.md` | Exact repository, branch and PR state |
| `CHANGELOG.md` | Chronological changes |
| `MANIFEST.md` | Live file index and integrity guidance |

## Validation snapshot

- **V0 Active Mission intake:** complete; M001 baseline confirmed.
- **V1 real Mission walkthrough:** ready to schedule; not yet passed.
- **V2 Mission lifecycle observation:** blocked until M001 is Committed after V1.
- **V3 generic Decision Record:** complete with prospective-decision limitation.
- **V4 role-view comprehension:** desk walkthrough complete; M001 real participant test pending.
- **V5 AI work control:** partial; A1/A2 and design-level A3 dry run complete, code/test and non-document sandbox work pending.
- **V6 authoritative-source map:** blocked by missing actual enterprise tool and owner map.

## Status model

- **Confirmed:** accepted and usable as a working constraint.
- **Candidate:** plausible direction that still requires evidence or a further gate.
- **Frozen:** formally approved stable baseline; changes require an explicit superseding decision.
- **Superseded:** replaced by an explicit authoritative supersession record but retained for traceability.
- **Missing:** a required fact is not available.
- **Unknown:** current state cannot be verified from accessible authority.
- **Unverified / Not authoritative:** a historical claim exists but lacks authoritative evidence; it is not automatically Superseded.

## Current next step

Prepare and run the M001 cross-functional walkthrough. The named business acceptance representative remains Missing and is a decision gate before final business acceptance. Keep Draft PR #1 open and unmerged.