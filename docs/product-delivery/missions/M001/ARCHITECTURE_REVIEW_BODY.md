# SmartQuote Permanent Architecture Review Body

Work Item: `SQT-ARCH-BODY-ACTIVATE-01`

## Permanent route
The permanent SmartQuote architecture-governance route is the **SmartQuote Architecture Review Body (ARB)**.

Seats:
- Product Authority: Jason Lin
- Engineering Authority: Ka Chen — seat not effective until `SQ-AUTH-003` is explicitly accepted and made effective
- Independent Review: Dorden, or another explicitly accepted independent reviewer if Dorden declines or is unavailable

## Scope
The ARB owns review/approval of:
- final technology baseline;
- material or hard-to-reverse architecture decisions;
- Shared Foundation bindings for Merchant Identity, Identity/Auth, Tenant, Secrets and Audit;
- material database/runtime topology changes;
- new external vendors or infrastructure classes;
- L2 architecture exceptions.

## Decision control
A material decision requires:
1. effective Engineering Authority participation;
2. Product Authority participation where product boundaries are affected;
3. independent review with no unresolved conflict;
4. exact decision object/evidence freeze;
5. documented Shared Foundation and trigger-deferred control impact.

No single participant may author, review and approve a material decision alone.

## Current status
`STRUCTURE APPROVED / NOT YET OPERATIONALLY EFFECTIVE`

Reason: the required Engineering Authority and independent-review seats still need attributable acceptance/effectiveness. Issue `STAR-SAAS/star-architecture#33` is the activation route.

This record does not pass Gate 2 or authorize Engineering Start.
