# STAR Decision Record Validation

**Version:** v0.1.0  
**Status:** Validation evidence; template remains candidate  
**Purpose:** Test whether one generic Decision Record can remain understandable across different decision domains before STAR creates specialized record types.

## Decisions tested

| Decision | Type used | Evidence file |
|---|---|---|
| `DEC-0030` — trace work to customer/user value and operational learning | Product / Delivery | `examples/decisions/DEC-0030_VALUE_TRACEABILITY.md` |
| `DEC-0032` — store the baseline in `star-architecture/docs/product-delivery/` | Architecture / Repository Governance | `examples/decisions/DEC-0032_GITHUB_BASELINE_LOCATION.md` |
| `DEC-0034` — plan multi-step work and report it step by step | Governance / Working Method | `examples/decisions/DEC-0034_STEPWISE_WORK_REPORTING.md` |

## Findings

### What worked across all three

The same structure remained understandable for:

- context and the problem requiring a decision;
- the chosen decision stated separately from rationale;
- options considered and why alternatives were rejected;
- expected benefits, accepted trade-offs and follow-up work;
- affected customers, products, Missions, systems and teams;
- validation evidence and revisit triggers;
- owner, status, effective date and supersession relationships.

No additional top-level field was required for any of the three decision types.

### Where proportionality is needed

- Low-impact decisions may use shorter option and impact sections.
- A decision may use more than one Type label when it crosses boundaries.
- “Not applicable” is preferable to deleting standard fields silently.
- High-risk legal, security, compliance or financial decisions may require additional evidence or approval records, but that has not yet demonstrated the need for a separate template.

### Limitation

These records were created retrospectively from already confirmed decisions. The structure has not yet been tested while a contested decision is actively being evaluated by multiple participants.

## Current conclusion

The generic `templates/DECISION_RECORD.md` is sufficient as the first STAR decision format.

Do **not** create separate ADR, PDR, BDR or GDR templates yet. Specialize only when a real decision demonstrates that a required field, workflow or authority model cannot be expressed clearly with the generic record and its Type field.

## V3 result

**Status:** Complete with limitation.

**Evidence:** three accepted decisions from different domains were documented using one template without structural failure.

**Next validation:** use the same template prospectively for one material decision before it is accepted, including disagreement, evidence review and approval.
