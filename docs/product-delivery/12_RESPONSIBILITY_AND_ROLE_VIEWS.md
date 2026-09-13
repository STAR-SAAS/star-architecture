# STAR Mission Responsibility and Role Views — Candidate

**Version:** v0.1.0  
**Status:** Candidate; not frozen  
**Purpose:** Make responsibility and first-view information clear without forcing every participant to read the full delivery model.

## Keep these terms separate

| Term | Meaning |
|---|---|
| **Value Receiver** | Person, organization or internal team expected to receive the outcome. |
| **Stakeholder** | Any party that affects, performs, governs, consumes or is affected by the Mission. |
| **Role** | A recurring responsibility pattern; it is not necessarily a job title. |
| **Contributor** | Human, team, AI agent or system that performs a Work Item. |
| **Mission Owner** | One accountable human for achieving and verifying the Mission outcome. |
| **Product / Service Owner** | Accountable human for the enduring product or service after the Mission closes. |
| **Approver** | Human with authority to accept a decision, risk or release within a defined boundary. |
| **Reviewer** | Party that evaluates quality, correctness, risk or evidence but may not own the outcome. |
| **Operator** | Party responsible for running, supporting or recovering the delivered capability. |
| **AI Agent** | A governed contributor that acts within an authorized task and context boundary. |
| **System** | An automated participant or authoritative source involved in the work. |

## Minimum accountability rules

1. Every Mission has exactly one accountable **Mission Owner**.
2. Enduring Product and Service ownership remains explicit after Mission closure.
3. One person may perform several roles; a role must not be confused with an organization chart.
4. AI agents may perform work, analysis and review, but do not hold executive, legal, compliance or high-risk approval accountability unless a later approved policy explicitly permits it.
5. Approval effort is proportional to customer, operational, security, compliance and financial impact.
6. Material high-risk work requires independent review; the producer should not be the sole approver.
7. External dependencies and accountable contacts are named rather than hidden inside a task list.

## What each participant sees first

| Participant | First questions the Mission view must answer | Expected contribution |
|---|---|---|
| **Customer / End User** | What problem is being solved? What changes? When? How is success accepted? | Feedback, usage evidence and acceptance input |
| **Leadership / Sponsor** | What value, risk, progress and decision require attention? | Direction, priority and accountable approval |
| **Product Manager / Owner** | Who needs what outcome? What is in and out? How will value be measured? | Scope, priority, acceptance and product follow-through |
| **Project / Delivery Manager** | Who depends on whom? What is blocked? What is the next milestone? | Coordination, dependency and delivery-state management |
| **Architect / Tech Lead** | What boundaries, constraints, decisions and system impacts matter? | Design constraints, decision records and technical coherence |
| **Frontend / Backend / Mobile / Data Engineering** | What Work Item, interface, acceptance and current context apply now? | Implementation, tests, review and linked technical evidence |
| **QA / Quality Engineering** | What behavior, risk and evidence must be verified? | Test strategy, execution evidence and defect assessment |
| **AI Team / Agent** | What authorized task, context, tools, limits and human reviewer apply? | Draft analysis, code, tests or documents within the assigned boundary |
| **DevOps / SRE / Operations / Support** | How is it released, observed, supported, rolled back and recovered? | Operational readiness, runbook, monitoring and incident feedback |
| **Security / Risk / Compliance / Legal / Finance** | What controlled impact, obligation and evidence requires review or approval? | Guardrails, approvals, exceptions and audit evidence |
| **Sales / Customer Success / Account Management** | What customer promise, communication and readiness are affected? | Customer context, expectation alignment and rollout communication |
| **Partner / Vendor / External Provider** | What dependency, contract, certification, support or deadline is required? | External readiness, deliverables and escalation contact |

## Mission responsibility card

Every Mission should be able to show this small card without opening a large RACI matrix:

- **Receives value:**
- **Mission Owner:**
- **Product / Service Owner:**
- **Decides / approves:**
- **Does the work:**
- **Reviews / validates:**
- **Operates / supports:**
- **Affected / informed:**
- **External dependencies and contacts:**
- **AI participation and human review boundary:**

## Stakeholder gap check

Before a Mission is committed, check whether it affects:

- customer, buyer, administrator or end user;
- prospect, sales, customer success, account management or support;
- product, project/delivery, design or research;
- architecture, frontend, backend, mobile, data, AI or technical writing;
- QA, release, operations, SRE, NOC or incident response;
- security, privacy, risk, compliance, legal, finance, procurement or audit;
- partner, vendor, bank, PSP, regulator, certification body or other external party;
- an authoritative system such as GitHub, CRM, issue tracking, CI/CD, monitoring or finance systems.

A category may be marked **Not affected**, but it should not be silently omitted.

## Validation status

This model is consistent with the current Stakeholder Map and Decision Log. It is a candidate answer to `OQ-005` and supports `OQ-010`, but it still requires walkthroughs using a real active Mission. The walkthrough should confirm that each participant can identify their next action without seeing irrelevant detail.
