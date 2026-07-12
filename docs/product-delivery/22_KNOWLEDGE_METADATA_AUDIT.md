# STAR Knowledge Metadata Audit

| Field | Value |
|---|---|
| **Type / scope** | Audit evidence — ownership and review metadata for Product Delivery knowledge |
| **Version / status** | v0.1.1 — Candidate audit evidence |
| **Owner** | STAR leadership |
| **Maintainer** | Product Delivery maintainers |
| **Last reviewed** | 2026-07-12 |
| **Review trigger** | New high-impact file, ownership gap, contradictory guidance, freeze proposal or real-Mission finding |
| **Authoritative working source** | This repository path in Draft PR #1; `main` only after approved merge |
| **Affects** | Durable Markdown, AI context reliability and knowledge lifecycle validation |
| **Supersession** | None |
| **Access** | Public |

## Purpose

Identify the minimum metadata needed to keep Product Delivery Markdown current, owned and safe for human and AI use, then verify that the highest-impact files apply it without adding unnecessary ceremony to every note.

## Minimum metadata candidate

Material, reusable or decision-bearing knowledge should identify:

| Field | Purpose |
|---|---|
| **Version** | Distinguishes meaningful revisions |
| **Status** | Candidate, Confirmed, Frozen, Superseded or Archived |
| **Owner** | Accountable human or maintained governance group |
| **Last reviewed** | Shows when correctness was last checked |
| **Review trigger / next review** | Prevents silent expiry |
| **Authoritative source** | Identifies where the current truth is maintained |
| **Related decisions / scope** | Shows why the item exists and what it affects |
| **Access classification** | Required when content is not public or contains restricted information |

Not every temporary note requires the full header. Apply it where stale or contradictory content could materially affect work.

## Repository audit

| Content group | Current strengths | Remaining gap | Priority |
|---|---|---|---|
| **Charter, Decision Log, Working Method** | Full metadata applied; decisions have IDs and explicit scope | Named individual/formal governance ownership before freeze | High |
| **Open Questions, Assumptions, Superseded Ideas** | States are separated and review ownership is covered by the central register | Aging interval and named resolution owners | High |
| **Research Canon** | Adoption posture and external sources are recorded | Source-verification date per entry and named maintainer | Medium-high |
| **Foundation, information and AI candidates** | Full metadata applied to the highest-impact candidates | Real-Mission and AI-work evidence | High |
| **Validation plan and Work Status** | Full metadata applied; update triggers are explicit | Validation owners for blocked real-world tests | High |
| **Validation evidence** | Date/status and findings are visible | Evidence owner on some retrospective records | Medium-high |
| **Mission and Decision templates** | Purpose and authoring rules are clear | Template version policy and named owner before organizational freeze | Medium |
| **Examples** | Clearly marked as examples | Expiry/review when they stop reflecting current practice | Medium |
| **README, Manifest, Changelog and Sync Status** | Provide navigation and live repository controls | Named repository maintainer before merge/freeze | High |

## Metadata hardening result

Full embedded metadata is now present in the priority files:

1. `00_PROJECT_CHARTER.md`;
2. `01_DECISION_LOG.md`;
3. `07_WORKING_METHOD.md`;
4. `11_FOUNDATION_CANDIDATE.md`;
5. `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md`;
6. `14_AI_WORK_GOVERNANCE.md`;
7. `15_VALIDATION_PLAN.md`;
8. `17_WORK_STATUS.md`.

`23_KNOWLEDGE_REVIEW_REGISTER.md` now records ownership, maintenance responsibility, status and review triggers for the wider high-impact repository set.

## Review triggers for this baseline

A review should occur when:

- a confirmed decision changes or is superseded;
- a real Mission exposes a missing or unnecessary field;
- a product, service, team or repository owner changes;
- a security, compliance, audit or incident finding affects the guidance;
- an external standard or linked tool changes materially;
- humans or AI receive contradictory instructions;
- a candidate is proposed for freeze;
- no review has occurred within the agreed interval once an interval is defined.

## Findings

1. The repository consistently separates Candidate, Confirmed and Frozen concepts.
2. The highest-impact files now expose owner/maintainer, review trigger, authoritative working source, scope and access.
3. A central register is more maintainable than adding a full header to every temporary note.
4. A governance group can maintain the working repository, but a named accountable human or approved governance body is still required before formal freeze.
5. Git history proves what changed, but not whether the current content is still correct; human ownership and review remain necessary.
6. Real-Mission and actual enterprise-system ownership remain unresolved and must not be invented.

## OQ-009 status

The minimum metadata, review triggers and repository review register now have a concrete candidate implementation. `OQ-009` remains open until named ownership and review behavior are tested during real Mission work and a material knowledge item is superseded or archived through the proposed lifecycle.
