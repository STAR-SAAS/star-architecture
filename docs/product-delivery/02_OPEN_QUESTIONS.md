# STAR Open Questions

**Version:** v0.1.3  
**Status:** Active

Open questions must not be presented as confirmed architecture.

## Priority A — blocks the next architecture baseline

| ID | Question | Why it matters | Current evidence / next validation |
|---|---|---|---|
| OQ-001 | What is STAR's final scope and name: Product Delivery system, capability system, engineering system, or broader operating system? | Prevents scope creep and unstable terminology. | Produce a one-page problem/value statement and compare alternatives after the Product Delivery foundation is tested. |
| OQ-002 | What is the minimum stable hierarchy from customer need/value to Mission and executable work? | Drives product, project and engineering traceability. | `11_FOUNDATION_CANDIDATE.md` proposes a minimum loop; populate `templates/MISSION_BRIEF.md` for one real active Mission. |
| OQ-003 | What is a Mission, exactly, and what is not a Mission? | "Mission" has been used as project, objective and work container. | A candidate definition, entry/exit boundaries and counterexamples now exist in `11_FOUNDATION_CANDIDATE.md`; validate size and closure on real work. |
| OQ-004 | Which objects are mandatory in the first implementation? | Avoids an overbuilt meta-model. | A six-object candidate exists in `11_FOUNDATION_CANDIDATE.md`; test whether a real Mission needs another top-level object. |
| OQ-005 | How should role, worker, team, stakeholder, owner and approver differ? | Needed for accountability, AI participation and permissions. | `12_RESPONSIBILITY_AND_ROLE_VIEWS.md` provides a candidate responsibility model; run a cross-functional walkthrough and identify ambiguity. |

## Priority B — repository and knowledge

| ID | Question | Why it matters | Current evidence / next validation |
|---|---|---|---|
| OQ-007 | What content belongs in GitHub versus issue tracking, CRM, monitoring, email/calendar and other systems? | Prevents GitHub from becoming a dumping ground. | `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md` proposes one authoritative source per information class; map STAR's actual tools and identify exceptions. |
| OQ-008 | What is the minimum decision-record taxonomy beyond ADR? | Product and governance decisions also need traceability. | `templates/DECISION_RECORD.md` tests one generic record with a Type field; apply it to one product, one architecture and one governance decision before specializing. |
| OQ-009 | How will knowledge be reviewed, expired and archived? | A growing repository without lifecycle control becomes unreliable. | A candidate lifecycle and minimum metadata exist in `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md`; apply owners and review triggers to current files. |

## Priority C — team experience and AI

| ID | Question | Why it matters | Current evidence / next validation |
|---|---|---|---|
| OQ-010 | What information should each role see first in a Mission view? | Supports fast comprehension without hiding necessary context. | Candidate views now exist in `12_RESPONSIBILITY_AND_ROLE_VIEWS.md` and `templates/MISSION_BRIEF.md`; test with PM, project manager, architect, FE, BE, QA, AI, Ops and customer participants. |
| OQ-011 | What are the authority and approval boundaries for AI agents? | AI participation without controls creates quality and security risk. | Candidate minimum limits appear in `12_RESPONSIBILITY_AND_ROLE_VIEWS.md`, `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md` and both templates; define human-required gates by risk class. |
| OQ-012 | How should context be assembled for AI tasks? | AI quality depends on current, relevant and authorized context. | Prototype a context package for one code or analysis Work Item. |
| OQ-013 | What onboarding targets are realistic for different roles? | Numeric targets such as 30 seconds, one hour or five days were proposed but not validated. | Test with actual team members. |

## Deferred

- Full knowledge graph or ontology technology
- Backstage adoption
- A2A production use
- Enterprise-wide capability map
- Commercial positioning of STAR OS

## Resolved questions

- **OQ-006:** Repository and path resolved by `DEC-0032`: `STARSAAS/star-architecture/docs/product-delivery/`.
