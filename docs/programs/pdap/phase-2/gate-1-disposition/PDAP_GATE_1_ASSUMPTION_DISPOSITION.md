# PDAP Gate 1 Assumption Disposition

## Approved for bounded Gate 1 use

### AA-05 · Technology-neutral observability outcomes

- Owner: Jason Lin.
- Implementation owner: future platform/infrastructure/operations owner.
- Scope: bounded Shared Foundation bootstrap and non-production first increment.
- Required outcomes: structured logs, correlation identifier, health signal, failure visibility, redaction and minimum audit evidence.
- Risk: tools may change and initial signals may be minimal.
- Validation trigger: first executable service or deployable artifact.
- Expiry: 2026-08-07 or approval of RFC-PLT-007, whichever occurs first.
- Reversal: replace tooling while preserving signal contracts.

AA-05 does not permit the absence of logs, health or failure evidence.

### AA-06 · Tool-neutral CI quality-control outcomes

- Owner: Jason Lin.
- Implementation owner: future application engineering owner.
- Scope: `star-platform` bounded bootstrap and non-production first increment.
- Required outcomes: repeatable build, unit-test execution, lint/static check, secret check, dependency visibility, artifact identity and explicit pass/fail evidence.
- Risk: CI provider and initial controls may later change.
- Validation trigger: first proposed engineering merge.
- Expiry: 2026-08-07 or approval of RFC-PLT-004, whichever occurs first.
- Reversal: replace CI tooling while retaining required checks and evidence.

AA-06 does not permit an engineering merge without actual checks and evidence.

## Other assumptions

- AA-01 through AA-04 continue within their approved scope and expiry.
- AA-07, AA-08 and AA-09 remain Candidate and are not approved for use.
- Assumptions cannot substitute for accepted engineering ownership, security boundaries, executable evidence or Gate passage.