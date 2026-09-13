# M001 SmartQuote Missing Authority — Leadership Decision-Ready Record

Status: **Explicit leadership dispositions required / No recommendation treated as decision**

Work Item: `SQT-AUTH-MISSING-DECISION-READY-01`

## Purpose

Provide one exact decision record for `SQ-AUTH-009` through `SQ-AUTH-017` so each route exits indefinite `Missing` through an explicit leadership disposition.

## Recommended decision set for current synthetic-only M1 scope

| Authority ID | Route | Recommended disposition | Boundary |
|---|---|---|---|
| `SQ-AUTH-009` | Business Acceptance Authority | Nominate now | Required before M1 business acceptance closes |
| `SQ-AUTH-010` | Architecture Authority | Nominate now or approved architecture review body | Required before final hard-to-reverse architecture / Gate 2 architecture commitment |
| `SQ-AUTH-011` | Finance / Pricing Authority | Trigger-deferred | Valid only while pricing/margin/financial values remain synthetic |
| `SQ-AUTH-012` | Risk Review Responsibility | Trigger-deferred | Must close before first risk-controlled decision |
| `SQ-AUTH-013` | Compliance Review Responsibility | Trigger-deferred | Must close before first compliance-controlled decision |
| `SQ-AUTH-014` | Security Review Responsibility | Trigger-deferred under current ceiling | Must close before protected data, credentials/access elevation, operated environments or production-bound security decisions |
| `SQ-AUTH-015` | Release Authority | Release-deferred | Mandatory before production Release |
| `SQ-AUTH-016` | Sales / workflow validation route | Nominate now or approve equivalent internal business-user route | Required for M1 internal-sales workflow evidence |
| `SQ-AUTH-017` | Channel Cost Accountable Contact | Trigger-deferred | Valid only while Channel Cost remains synthetic |

## Leadership decision fields

For every Authority ID record:

- `Leadership disposition`: Nominate named holder / Nominate governing body / Trigger-deferred / Release-deferred / Out of M001 first-stage scope / HOLD
- `Holder/body` where nominated
- `Trigger / defer boundary` where deferred
- `Conflict / independence conditions`
- `Decision date/time`

Any newly nominated holder still requires explicit acceptance and, where applicable, a separate Effectiveness Decision.

## Current result

Issue #28 contains recommendations and execution-status comments only; no explicit leadership disposition has yet been recorded. Therefore `SQ-AUTH-009` through `SQ-AUTH-017` remain unresolved.

## Non-effects

This record appoints nobody, resolves no route by itself, passes no M1/Gate 2, grants no Product Commitment, authorizes no Engineering Start, real commercial rules, real data, environment, deployment, Release or AI merge.
