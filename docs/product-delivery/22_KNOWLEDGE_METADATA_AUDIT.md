# STAR Knowledge Metadata Audit

**Version:** v0.1.0  
**Status:** Candidate audit evidence  
**Date:** 2026-07-12  
**Purpose:** Identify the minimum metadata needed to keep Product Delivery Markdown current, owned and safe for human and AI use.

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

## Current repository audit

| Content group | Current strengths | Main metadata gap | Priority |
|---|---|---|---|
| **Charter, Decision Log, Working Method** | Version and status are visible; decisions have IDs | Named maintainer, review trigger and formal effective scope | High |
| **Open Questions, Assumptions, Superseded Ideas** | States are clearly separated | Named owner for resolution/review and aging trigger | High |
| **Research Canon** | Adoption posture and external sources are recorded | Source-verification date per entry and maintainer | Medium-high |
| **Foundation, responsibility, information and AI candidates** | Candidate status is explicit | Owner, last review, review trigger and affected scope | High |
| **Validation evidence** | Date/status and findings are generally visible | Evidence owner and relationship to the validation register | Medium-high |
| **Mission and Decision templates** | Purpose and authoring rules are clear | Template owner, version policy and review trigger | Medium |
| **Examples** | Clearly marked as examples | Evidence date/source and explicit expiry when the example no longer reflects current practice | Medium |
| **README, Manifest, Changelog, Sync and Work Status** | Provide navigation and live status | Repository maintainer and update trigger | High |

## Priority files for metadata hardening

Apply the full minimum header first to:

1. `00_PROJECT_CHARTER.md`;
2. `01_DECISION_LOG.md`;
3. `07_WORKING_METHOD.md`;
4. `11_FOUNDATION_CANDIDATE.md`;
5. `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md`;
6. `14_AI_WORK_GOVERNANCE.md`;
7. `15_VALIDATION_PLAN.md`;
8. `17_WORK_STATUS.md`.

These files influence the largest number of later decisions and AI context packages.

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
2. Version and status are present on most important files, but ownership and review triggers are not yet consistent.
3. Adding metadata to every short note would create ceremony; apply it first to authoritative and high-impact files.
4. A missing owner is more dangerous than a missing review date: unowned knowledge must not remain silently authoritative.
5. Git history proves what changed, but not whether the current content is still correct; human ownership and review remain necessary.

## OQ-009 status

The minimum metadata and review triggers now have a concrete candidate answer. `OQ-009` remains open until owners and review triggers are applied to the priority files and tested during real Mission work.
