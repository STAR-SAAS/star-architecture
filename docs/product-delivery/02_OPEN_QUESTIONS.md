# STAR Open Questions

**Version:** v0.1.5  
**Status:** Active

Open questions must not be presented as confirmed architecture.

## Priority A — blocks the next architecture baseline

| ID | Question | Why it matters | Current evidence / next validation |
|---|---|---|---|
| OQ-001 | What is STAR's final scope and name: Product Delivery system, capability system, engineering system, or broader operating system? | Prevents scope creep and unstable terminology. | Produce a one-page problem/value statement and compare alternatives after the Product Delivery foundation is tested. |
| OQ-002 | What is the minimum stable hierarchy from customer need/value to Mission and executable work? | Drives product, project and engineering traceability. | `11_FOUNDATION_CANDIDATE.md` proposes a minimum loop; `16_ACTIVE_MISSION_INTAKE.md` shows the real data still missing. Populate one authoritative Mission Brief. |
| OQ-003 | What is a Mission, exactly, and what is not a Mission? | "Mission" has been used as project, objective and work container. | A candidate definition and counterexamples exist in `11_FOUNDATION_CANDIDATE.md`; validate size, hierarchy and closure on real work. |
| OQ-004 | Which objects are mandatory in the first implementation? | Avoids an overbuilt meta-model. | A six-object candidate exists in `11_FOUNDATION_CANDIDATE.md`; test whether a real Mission needs another top-level object. |
| OQ-005 | How should role, worker, team, stakeholder, owner and approver differ? | Needed for accountability, AI participation and permissions. | `12_RESPONSIBILITY_AND_ROLE_VIEWS.md` provides the candidate model and `20_ROLE_VIEW_DESK_WALKTHROUGH.md` passed a desk walkthrough. Validate with real participants. |

## Priority B — repository and knowledge

| ID | Question | Why it matters | Current evidence / next validation |
|---|---|---|---|
| OQ-007 | What content belongs in GitHub versus issue tracking, CRM, monitoring, email/calendar and other systems? | Prevents GitHub from becoming a dumping ground. | `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md` proposes one authoritative source per information class; map STAR's actual tools and owners. |
| OQ-008 | What is the minimum decision-record taxonomy beyond ADR? | Product and governance decisions also need traceability. | `18_DECISION_RECORD_VALIDATION.md` shows one generic template worked retrospectively across three domains. Test it prospectively on one contested or high-risk decision before closing this question. |
| OQ-009 | How will knowledge be reviewed, expired and archived? | A growing repository without lifecycle control becomes unreliable. | `22_KNOWLEDGE_METADATA_AUDIT.md` defines minimum metadata, priority files and review triggers. Apply the metadata to high-impact files and test ownership during real work. |

## Priority C — team experience and AI

| ID | Question | Why it matters | Current evidence / next validation |
|---|---|---|---|
| OQ-010 | What information should each role see first in a Mission view? | Supports fast comprehension without hiding necessary context. | `20_ROLE_VIEW_DESK_WALKTHROUGH.md` supports Why/What/Who/Now/Evidence for orientation. Test comprehension with real participants using an authoritative Mission. |
| OQ-011 | What are the authority and approval boundaries for AI agents? | AI participation without controls creates quality and security risk. | `14_AI_WORK_GOVERNANCE.md`, `19_AI_WORK_CONTROL_DRY_RUN.md` and `21_AI_CONTEXT_PACKAGE_TEST.md` validate A1/A2 documentation/GitHub work. Code/test and A3 dry-run remain open. |
| OQ-012 | How should context be assembled for AI tasks? | AI quality depends on current, relevant and authorized context. | `templates/AI_CONTEXT_PACKAGE.md` and `21_AI_CONTEXT_PACKAGE_TEST.md` provide and validate a minimum A2 package. Test it next on one code/test or non-document analysis Work Item. |
| OQ-013 | What onboarding targets are realistic for different roles? | Numeric targets such as 30 seconds, one hour or five days were proposed but not validated. | Test with actual team members. |

## Deferred

- Full knowledge graph or ontology technology
- Backstage adoption
- A2A production use
- Enterprise-wide capability map
- Commercial positioning of STAR OS

## Resolved questions

- **OQ-006:** Repository and path resolved by `DEC-0032`: `STARSAAS/star-architecture/docs/product-delivery/`.
