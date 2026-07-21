# STAR Company Governance Authority Model

| Field | Value |
|---|---|
| Status | Candidate |
| Leadership decision | Confirmed adoption for design use |
| Policy effective status | Not Effective |
| Named appointments | None |
| Authority-holder appointments | None |
| Source | DSP-001-047 and DSP-001-048 |
| Last reviewed | 2026-07-21 |

## Purpose

Define how STAR distinguishes decision Authority from organizational role, technical permission, execution and review. This Candidate model supports later Product, Architecture, Engineering, Risk, Compliance, Release and AI Governance design.

## Core principles

1. Authority belongs only to a governed human or governing body; AI tools cannot hold company decision Authority.
2. Accountability cannot be delegated away, even when execution is delegated.
3. System permission does not create Authority.
4. Missing Authority stops the decision and cannot be inferred by AI.
5. Temporary Authority requires exact scope, evidence, effective date, expiry and revocation.
6. Professional truth remains in the professional Source of Record.
7. High-risk decisions require appropriate independence and four-eyes.

## Authority hierarchy

```text
Founder / CEO Authority
→ Executive Leadership Authority
→ Portfolio and Corporate Governance Authority
→ Product / Architecture / Engineering / Risk / Compliance / Finance / Security Authority
→ Mission / Operations / QA / Release / Incident / Records Authority
→ Execution Assignments and Technical Permissions
```

The hierarchy does not remove professional hard-block or independent-review duties.

## Confirmed role boundaries

- Product Authority owns product intent, scope and business outcome.
- Mission Authority owns coordination, dependencies, evidence and readiness.
- Mission Authority cannot alone change Product Intent, pass a Gate or authorize Delivery.
- Architecture Authority does not automatically hold Engineering or Release Authority.
- Engineering Authority does not automatically hold Product, Commercial, Risk or Compliance Authority.
- Reviewer is not automatically Approver.
- Executor is not Accountable Owner.
- Technical administrator is not automatically the approver of their own access or change.

## Mandatory four-eyes baseline

Four-eyes is mandatory for:

- Material Pricing Rule;
- Channel Cost;
- Financial Exception;
- Compliance Exception;
- Production Release;
- Security Control;
- Access Elevation;
- Confidential or Restricted AI Use;
- Production Data Access;
- Policy Activation.

## Non-bypassable boundaries

Temporary assumptions and Founder-led Fast Track cannot bypass:

- law or regulatory prohibition;
- customer or merchant data confidentiality;
- credential and secret protection;
- core Tenant Isolation;
- KYC or AML obligations;
- explicit customer contract restrictions;
- Production Release Authority;
- unresolved Critical Security Risk.

## Emergency Authority

Emergency Authority is limited to temporary containment. Every use requires:

- exact scope;
- start time;
- expiry;
- notification recipients;
- evidence;
- retrospective review;
- restoration or revocation decision.

Emergency Authority never becomes continuing Authority automatically.

## Founder-led Fast Track exit boundary

Founder-led Fast Track ends before:

- policy activation;
- formal appointment;
- Product Commitment;
- Gate passage;
- Engineering Start;
- real sensitive-data use;
- production environment creation or use;
- external customer use;
- material financial decision;
- legal or compliance professional judgment.

## Authority acceptance mechanism — Candidate

A continuing Authority becomes valid only after all conditions are satisfied:

1. leadership formally designates the Authority;
2. the designated person explicitly accepts;
3. scope and accountability are recorded;
4. conflicts and independence are checked;
5. the Source of Record is established;
6. effective date is recorded;
7. expiry or review trigger is recorded;
8. required access is verified separately;
9. replacement and revocation mechanisms are established.

Holding an organizational title, repository permission or execution assignment does not by itself satisfy these conditions.

## Current workstream effects

### PORT-001

- Authority design may continue.
- Draft PR #2 remains Open / Draft / Unmerged.
- Independent Review remains Leadership-deferred / Not Passed.
- Freeze and Merge remain unauthorized.

### PORT-002

- AI Governance Authority cannot replace Product, Risk, Compliance, Security or Release Authority.
- Confidential or Restricted AI use and Employee AI Use Policy activation require four-eyes.
- Interim Controls remain unchanged.
- Package A, Wave A, Policy and PILOT-001 status remain unchanged.

### PORT-003

- Product and Mission Authority boundaries apply.
- Mission coordination cannot override Product Intent.
- M1, Gate 2, Product Commitment and Delivery each require separate decisions.
- Channel Cost, Pricing, Risk, Compliance and Architecture Authority remain to be confirmed.
- Current Product Intent and core-object design may continue within existing authority.

## Limitations

This Candidate model does not:

- appoint any person;
- activate any policy;
- grant system access;
- pass any Gate;
- authorize Engineering Start, Delivery, Release or production use;
- create monetary, pricing, risk or duration thresholds;
- replace Legal, Compliance, Finance, Security or Engineering professional judgment.

## Supersession

Any change requires a new global Decision Record identifying the changed provision, scope, effective use, non-effects and transition treatment.