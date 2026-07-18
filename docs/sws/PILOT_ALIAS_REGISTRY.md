# SWS Pilot Alias Registry

| Field | Value |
|---|---|
| **Registry status** | Pilot Candidate — DSP-003-005 controlled implementation |
| **Repository / branch** | `STAR-SAAS/star-architecture` / `agent/sws-pilot-package-b-m001-context` |
| **Alias owner** | Robin |
| **Human execution / content preparation responsibility** | Allen Liao — prepares controlled Package B content and evidence only; this does not grant Repository Write, publishing, approval or merge authority |
| **Normal authorized publishing maintainer** | Robin Koh / `rkoh-star` |
| **Modification approver** | Jason Lin |
| **Independent reviewer** | Dorden |
| **Authenticated publishing account** | `STARSAAS` under leadership-approved operational exception |
| **Exception scope** | DSP-003-005 only |
| **Exception expiry** | Child PR merge or Dispatch closure |
| **Last verified** | 2026-07-18 (Asia/Singapore) |

## Active entries

| Alias | Scope ID | Scope name | Project | Exact professional conversation | Repository | Authoritative branch | State |
|---|---|---|---|---|---|---|---|
| `M001` | `PORT-003` | Mission-001 · SmartQuote Foundation | `STAR OS` | `🚀 Mission-001 · SmartQuote Foundation` | `STAR-SAAS/star-architecture` | `agent/star-os-product-delivery-baseline` | Active Pilot Candidate |

## Resolution rule

- The exact literal Alias `M001` maps to exactly one active Scope: `PORT-003 · Mission-001 · SmartQuote Foundation`.
- Resolution reads this Registry. It must not infer an Alias from chat history, AI memory, approximate spelling, title similarity or prior conversations.
- Variants such as `m001`, `Mission 001` or `SmartQuote Mission` are not aliases unless separately approved and recorded.

## Collision control

A collision exists when:

- the same exact Alias maps to more than one active Scope;
- another active entry uses `M001`;
- the Alias entry, Context Package and authoritative Mission record disagree on Scope, Project, conversation, repository or branch;
- a deprecated Alias is treated as active;
- an unresolved migration or tombstone conflicts with the active entry.

On collision:

1. stop resolution before loading the Context Package;
2. set the affected Package state to `Blocked`;
3. preserve the last verified Registry commit and blob SHA;
4. record the conflicting entries and authoritative sources;
5. Allen Liao prepares the smallest correction as human execution / content preparation work only;
6. Robin confirms the correct M001 Scope;
7. Dorden performs independent review;
8. Jason Lin approves the modification;
9. Robin Koh / `rkoh-star`, or an explicitly approved operational exception account, performs authorized publishing;
10. restore the prior lifecycle state only after verified correction.

AI must not choose a likely mapping.

## Modification workflow

1. Robin proposes or confirms the M001 Alias meaning.
2. Allen Liao prepares a minimal content correction and evidence package; this does not grant Repository Write, publishing, approval or merge authority.
3. The change records old value, new value, reason, actor, source, timestamp and recovery point.
4. Dorden independently reviews uniqueness, provenance, collision handling and non-target impact.
5. Robin confirms the resulting M001 Scope mapping.
6. Jason Lin approves the modification and Report Back.
7. Robin Koh / `rkoh-star`, or an explicitly approved operational exception account, performs authorized publishing.
8. The approved change may be merged only after all required gates are satisfied.

## Migration, deprecation and exit

- **Migration:** preserve the prior entry and provenance; create a redirect only after the new target and fingerprints are verified.
- **Deprecation:** retain the entry as a tombstone with deprecation reason, date and replacement pointer or explicit no-replacement state.
- **Reuse:** a deprecated Alias must not be silently reused.
- **Pilot exit:** leadership explicitly chooses `retain`, `migrate` or `deprecate` before Pilot closure.

## Authority boundary

This Registry does not grant Allen Liao Repository Write, publishing, approval or merge authority. It does not pass M1, mark M001 Committed, authorize SmartQuote Delivery, approve product scope or architecture, or replace the authoritative M001 Decision Log and Work Status.