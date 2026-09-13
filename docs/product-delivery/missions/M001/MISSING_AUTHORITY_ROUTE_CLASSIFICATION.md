# M001 · SmartQuote Missing Authority / Professional Route Classification

Status: **Prepared Decision Classification / No holder appointed**

Work Item: `SQT-AUTH-MISSING-ROUTES-01`

## Purpose

Separate the nine currently Missing Authority / professional-responsibility routes by the controlled action they actually block. This avoids treating every Missing route as an identical immediate Engineering Start blocker while preserving mandatory controls when their trigger is reached.

## Proposed classification for leadership decision

| Authority ID | Route | Proposed blocking class | Earliest controlled action blocked | Current state |
|---|---|---|---|---|
| `SQ-AUTH-009` | Business Acceptance Authority | **M1 blocker** | M1 business acceptance / business acceptance evidence | Missing |
| `SQ-AUTH-010` | Architecture Authority | **Gate 2 / hard-to-reverse architecture blocker** | final architecture commitment; Gate 2 architecture disposition; material hard-to-reverse design | Missing |
| `SQ-AUTH-011` | Finance / Pricing Authority | **Real-commercial-rule blocker** | real pricing, margin, financial thresholds/exceptions; any material financial rule activation | Missing |
| `SQ-AUTH-012` | Risk Review Responsibility | **Trigger-based controlled-decision blocker** | risk-controlled decision when risk review is triggered | Missing |
| `SQ-AUTH-013` | Compliance Review Responsibility | **Trigger-based controlled-decision blocker** | compliance-controlled decision when compliance review is triggered | Missing |
| `SQ-AUTH-014` | Security Review Responsibility | **Security / protected-data / access-control blocker** | material Security Control, protected/real data, credential/access elevation, production security disposition | Missing |
| `SQ-AUTH-015` | Release Authority | **Release-only blocker** | production Release | Missing |
| `SQ-AUTH-016` | Sales Representative | **M1 workflow-validation blocker** | representative internal-sales workflow validation / acceptance evidence | Missing |
| `SQ-AUTH-017` | Channel Cost Accountable Contact | **Real Channel Cost blocker** | real Channel Cost source/effective-date governance and downstream pricing use | Missing |

## Interpretation

### Required before M1 can close

- `SQ-AUTH-009` Business Acceptance Authority.
- `SQ-AUTH-016` Sales Representative or an explicitly approved equivalent business-user validation route.

M1 may continue to prepare synthetic evidence before these are named, but M1 should not be represented as Passed without an accepted business-validation route.

### Required before Gate 2 / hard-to-reverse architecture commitment

- `SQ-AUTH-010` Architecture Authority.

Architecture options/ADRs may be prepared before appointment; final architecture commitment should not be represented as professionally approved until the route is closed.

### Required before real commercial rules / inputs

- `SQ-AUTH-011` Finance / Pricing Authority.
- `SQ-AUTH-017` Channel Cost Accountable Contact.

Synthetic pricing, Channel Cost and approval examples may continue as preparation. No real thresholds, margin rules, Channel Cost values or material financial exceptions should be activated without these routes.

### Trigger-based routes

- `SQ-AUTH-012` Risk.
- `SQ-AUTH-013` Compliance.
- `SQ-AUTH-014` Security.

These routes should be resolved no later than the first controlled action that triggers them. They should not be silently waived because the early work is synthetic/documentation-only. Security is expected to become material before protected data, credentials, access elevation, environment operation or production-bound controls.

### Required before Release, not necessarily before bounded pre-release preparation

- `SQ-AUTH-015` Release Authority.

Release Authority remains mandatory before production Release. Its absence should not be misrepresented as preventing every documentation, architecture-option or synthetic-test preparation task.

## Leadership decisions still required

For each Missing route, leadership must choose one of:

1. **Nominate now** — identify a candidate holder, obtain explicit acceptance, resolve conflict/independence, then issue separate Effectiveness Decision.
2. **Defer to explicit trigger** — only where this record classifies the route as trigger-based or Release-only; record the trigger and latest closure point.
3. **Use approved governing body / independent reviewer route** — only if company governance permits the scope and the body/individual explicitly accepts it.
4. **Hold** — if no acceptable route exists.

No individual is nominated by this classification record.

## Current recommendation

- Close `SQ-AUTH-009`, `SQ-AUTH-010`, and `SQ-AUTH-016` as the first missing-route batch because they directly affect M1/Gate 2 progression.
- Prepare `SQ-AUTH-011` and `SQ-AUTH-017` in parallel so technology/product decisions do not outrun commercial SoR governance.
- Bind explicit triggers for `SQ-AUTH-012`, `013`, `014`, and `015` rather than falsely marking them resolved.

## Non-effects

This classification appoints nobody, records no acceptance, makes no Authority effective, passes no Gate, grants no Product Commitment, authorizes no Engineering Start, real data, commercial-rule activation, environment, deployment or Release.
