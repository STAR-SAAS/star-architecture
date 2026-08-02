# SWS-001 · Scope Alias Registry Pilot

| Field | Value |
|---|---|
| Status | Pilot |
| Owner | STAR Architecture maintainers |
| Last verified | 2026-07-21 against Draft PR #2 working records |
| Scope | Minimal verified aliases for governed context loading |
| Classification | Public-safe |

## Rules

1. An Alias must resolve exactly and uniquely.
2. Alias collision stops resolution and marks the loading attempt Blocked.
3. Chat history and AI memory cannot create or infer aliases.
4. An Alias cannot be silently reused for another Scope.
5. A renamed Scope retains a Deprecated entry or Tombstoned entry with provenance.
6. The Registry identifies where governed context should be loaded; it does not determine professional truth or status.
7. Professional status remains in the authoritative professional source.
8. Sensitive locations, private mappings, markers and credentials are prohibited.
9. New entries require source verification and bounded review.

## Registry

| Alias | Scope ID | Professional Project | Professional Conversation | Authoritative source | Status | Collision rule | Owner | Last verified | Notes |
|---|---|---|---|---|---|---|---|---|---|
| M001 | PORT-003 · Mission-001 SmartQuote Foundation | STAR OS | 🚀 Mission-001 · SmartQuote Foundation | `STAR-SAAS/star-architecture`, Draft PR #1, `docs/product-delivery/missions/M001/` | Active | Stop resolution and mark Blocked if another active entry uses `M001` or if the source cannot be resolved uniquely | STAR Architecture maintainers | 2026-07-21 from verified portfolio and M001 coordination records | Resolves the loading destination only; M1, Commitment and Delivery state remain in professional records |

## Lifecycle

- `Pilot`: Registry mechanism is under validation.
- `Active`: Alias may be used within the Pilot after successful exact resolution.
- `Deprecated`: Alias remains resolvable only to a migration notice and replacement Alias.
- `Tombstoned`: Alias must not resolve to an active Scope and retains historical provenance.

## Stop conditions

Stop and report a finding when:

- more than one active entry matches an Alias;
- the professional source is Missing, Stale or inaccessible;
- a proposed entry depends only on chat memory;
- a proposed entry exposes private information;
- a Scope rename would silently reuse an existing Alias;
- resolution would be used to infer professional status.

This Pilot does not authorize automatic context synchronization, product work, policy activation, Gate passage, Product Commitment, Delivery start, Freeze or Merge.
