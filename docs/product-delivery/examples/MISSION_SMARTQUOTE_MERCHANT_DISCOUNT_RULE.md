# Example Mission — SmartQuote Merchant Discount Rule

**Status:** Example only; not an active commitment  
**Purpose:** Show how a team-facing Mission Brief can remain concise while linking deeper detail.

> Deliver configurable merchant-specific discount rules so quotation users can create accurate, auditable quotes with less manual handling.

| Field | Value |
|---|---|
| **Mission ID** | EX-MIS-SQ-001 |
| **Mission Owner** | TBD before commitment |
| **Product / Service Owner** | SmartQuote Product Owner — TBD |
| **Target date** | TBD |
| **Risk level** | Medium candidate |

## Why

- **Value receiver:** merchant quotation user and merchant business.
- **Problem:** negotiated discounts are applied manually or inconsistently.
- **Why now:** manual handling increases quotation time, pricing error and audit risk.
- **Expected outcome:** authorized users can apply the correct configurable discount rule and understand the resulting price.
- **Measures:** quotation preparation time, pricing-error rate, manual exception rate, user adoption and post-release incidents.

## What

### In scope

- merchant-specific configurable discount rules;
- precedence and validity rules;
- authorization or approval where required;
- calculation, quote display and audit trail;
- API/data changes, tests, rollout and support guidance.

### Out of scope

- redesigning the complete pricing engine;
- unrelated promotional campaigns;
- automatic commercial approval outside agreed authority.

### Acceptance evidence

- agreed business examples calculate correctly;
- unauthorized users cannot create or apply restricted rules;
- API and UI expose a clear result and error state;
- audit evidence records rule, version and actor;
- regression and rollout evidence is available;
- pilot users confirm the outcome is usable.

## Who

- **Mission Owner:** TBD.
- **Product:** defines business rule, scope and success evidence.
- **Project / Delivery:** coordinates dependencies, milestone and blockers.
- **Architecture / Tech Lead:** confirms pricing boundary, configuration, precedence and audit design.
- **Backend:** implements rule evaluation, API and persistence changes.
- **Frontend:** implements configuration/display, permissions and error handling where needed.
- **QA:** verifies examples, edge cases, permissions and regression.
- **AI:** may draft rules analysis, code, tests and documentation under human review.
- **Operations / Support:** prepares rollout, monitoring and customer explanation.
- **Finance / Compliance:** reviews discount authority and audit requirements where applicable.

## Now

- **Current state:** example; not started.
- **Next actions before commitment:**
  1. name Mission and Product Owners;
  2. confirm real merchant/user examples and approval boundaries;
  3. identify current pricing sources, interfaces and rollout target.
- **Key risks:** conflicting rule precedence, unauthorized discounts, stale configuration and incorrect rounding/currency behavior.
- **Decisions needed:** canonical precedence model; effective-date/version behavior; approval threshold.

## Delivery and evidence

- **Release path:** development → automated tests → staging/UAT → controlled pilot → wider rollout.
- **Operational evidence:** rule failures, manual overrides, pricing errors and adoption metrics.
- **Closure condition:** released and operationally supported, with acceptance evidence reviewed and delayed business measures assigned to an owner/date.

## Linked detail

To be linked when this becomes active: business rules, Decision Records, API/data contracts, code/PRs, tests, monitoring, rollout and customer feedback.

## Template finding

The Mission Brief can describe this change without making PRD, architecture, API or test documents top-level layers. The unresolved gap is not another document type; it is the absence of real owners, examples, authority limits and current-system links.