# M001 SmartQuote Missing Authority / Professional Route Decision Sheet

Status: **Leadership decision required / No holder inferred**

Work Item: `SQT-AUTH-MISSING-ROUTES-02`

## Purpose

Turn the nine remaining Missing routes into explicit decision choices rather than leaving them indefinitely unclassified.

## Decision options

For each route leadership must choose one of:

- `Nominate named holder`
- `Nominate governing body / review panel`
- `Trigger-deferred`
- `Release-deferred`
- `Out of M001 first-stage scope`
- `HOLD`

A defer option is valid only where the controlled action is not yet triggered and the deferral itself does not undermine M1/Gate 2.

## Required decisions

| Authority ID | Route | Current blocking point | Recommended next disposition | Leadership decision |
|---|---|---|---|---|
| `SQ-AUTH-009` | Business Acceptance Authority | M1 / business acceptance | Nominate now | Pending |
| `SQ-AUTH-010` | Architecture Authority | hard-to-reverse architecture / Gate 2 | Nominate now or approved governing body | Pending |
| `SQ-AUTH-011` | Finance / Pricing Authority | real pricing / margin / financial thresholds | May be trigger-deferred if M1 uses synthetic rules only | Pending |
| `SQ-AUTH-012` | Risk Review Responsibility | risk-controlled decisions | Trigger-deferred unless M1 explicitly triggers risk judgment | Pending |
| `SQ-AUTH-013` | Compliance Review Responsibility | compliance-controlled decisions | Trigger-deferred unless M1 explicitly triggers compliance judgment | Pending |
| `SQ-AUTH-014` | Security Review Responsibility | material security controls / protected data / production access | Nominate for architecture/security baseline or trigger-defer with explicit boundary | Pending |
| `SQ-AUTH-015` | Release Authority | production Release | Release-deferred | Pending |
| `SQ-AUTH-016` | Sales Representative / workflow validation route | M1 workflow validation | Nominate now or approve an equivalent internal business-user route | Pending |
| `SQ-AUTH-017` | Channel Cost Accountable Contact | real Channel Cost / pricing input governance | Trigger-deferred while synthetic-only; required before real commercial data | Pending |

## Decision rule

- `SQ-AUTH-009`, `010`, and an approved `016` validation route are the highest-priority missing routes for M1/Gate 2 closure.
- `011` and `017` need not block purely synthetic M1 evidence if real pricing/channel-cost decisions remain explicitly prohibited.
- `012`–`014` may be trigger-based, but any triggered controlled decision must stop until the professional route is effective.
- `015` is a Release-stage blocker and must not be misrepresented as an early documentation blocker.

## Non-effects

This sheet does not nominate any person, appoint any Authority, make any route Effective, pass M1/Gate 2, grant Product Commitment, authorize Engineering Start, or authorize implementation, real data, environment, deployment, Release or AI merge.
