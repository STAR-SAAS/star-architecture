# STAR Open Questions

**Version:** v0.1.0  
**Status:** Active

Open questions must not be presented as confirmed architecture.

## Priority A — blocks the next architecture baseline

| ID | Question | Why it matters | Next validation |
|---|---|---|---|
| OQ-001 | What is STAR's final scope and name: Product Delivery system, capability system, engineering system, or broader operating system? | Prevents scope creep and unstable terminology. | Produce a one-page problem/value statement and compare alternatives. |
| OQ-002 | What is the minimum stable hierarchy from customer need/value to Mission and executable work? | Drives product, project and engineering traceability. | Test on one SmartQuote and one GateHub change. |
| OQ-003 | What is a Mission, exactly, and what is not a Mission? | "Mission" has been used as project, objective and work container. | Define entry/exit criteria and counterexamples. |
| OQ-004 | Which objects are mandatory in the first implementation? | Avoids an overbuilt meta-model. | Identify the minimum objects needed for one end-to-end delivery. |
| OQ-005 | How should role, worker, team, stakeholder, owner and approver differ? | Needed for accountability, AI participation and permissions. | Create a small responsibility and authority model. |

## Priority B — repository and knowledge

| ID | Question | Why it matters | Next validation |
|---|---|---|---|
| OQ-006 | Should `STARSAAS/star-architecture` be the authoritative GitHub home for this baseline, or should a dedicated STAR OS repository be created? | Determines ownership and future folder boundaries. | Executive repository decision. |
| OQ-007 | What content belongs in GitHub versus issue tracking, CRM, monitoring, email/calendar and other systems? | Prevents GitHub from becoming a dumping ground. | Define authoritative source by information class. |
| OQ-008 | What is the minimum decision-record taxonomy beyond ADR? | Product and governance decisions also need traceability. | Compare one generic Decision Record with typed variants. |
| OQ-009 | How will knowledge be reviewed, expired and archived? | A growing repository without lifecycle control becomes unreliable. | Define owner, review date and supersession rules. |

## Priority C — team experience and AI

| ID | Question | Why it matters | Next validation |
|---|---|---|---|
| OQ-010 | What information should each role see first in a Mission view? | Supports fast comprehension without hiding necessary context. | Run role walkthroughs for PM, project manager, architect, FE, BE, QA, AI, Ops and customer. |
| OQ-011 | What are the authority and approval boundaries for AI agents? | AI participation without controls creates quality and security risk. | Define human-required gates by risk class. |
| OQ-012 | How should context be assembled for AI tasks? | AI quality depends on current, relevant and authorized context. | Prototype context package for one code change. |
| OQ-013 | What onboarding targets are realistic for different roles? | Numeric targets such as 30 seconds, one hour or five days were proposed but not validated. | Test with actual team members. |

## Deferred

- Full knowledge graph or ontology technology
- Backstage adoption
- A2A production use
- Enterprise-wide capability map
- Commercial positioning of STAR OS
