# STAR Conversation Governance

| Field | Value |
|---|---|
| Document ID | SWS-CG-001 |
| Version / status | v0.1.0 — Working baseline; not frozen |
| Owner | STAR leadership |
| Maintainer | STAR Architecture maintainers |
| Scope | All STAR conversations and supporting AI tools |
| Decision references | GWR-01–12; SWS-DEC-005–009; proposed SWS-DEC-010–012 |

## 1. Purpose

STAR conversations are scoped execution spaces, not authoritative memory stores. This baseline defines how conversations are routed, resumed, transferred and closed without requiring the user to reconstruct prior context.

## 2. Conversation scope and ownership

Every material conversation declares:

- Project and conversation name;
- professional scope and objective;
- accountable human owner;
- authoritative repositories or systems;
- permitted AI/tool mode;
- current lifecycle status;
- decision and escalation boundary.

The conversation owner maintains scope clarity, current status and handoff quality. The initiating AI or human owns the Bootstrap check. Accountable business, product, governance or technical decisions remain with named humans.

A conversation may execute work only inside its declared scope. Cross-scope work is routed rather than silently absorbed.

## 3. Conversation Contract

At start or material scope change, establish a concise Contract containing:

1. destination Project and conversation;
2. objective and value receiver;
3. in-scope and out-of-scope work;
4. authoritative sources;
5. expected artifacts or result;
6. execution mode;
7. escalation conditions;
8. required durable records;
9. completion or handoff condition.

The full template is `STAR_CONVERSATION_CONTRACT_TEMPLATE.md`.

## 4. Routing Gate

Before material execution, answer:

1. Is this the correct Project?
2. Is this the correct professional conversation?
3. Is the current Chat, Work or Codex mode suitable?
4. Does another scope own the authoritative result?
5. Is the work orchestration or professional execution?

Outcomes:

- **Proceed** — scope and mode match.
- **Proceed with brief warning** — work is safe but mode is suboptimal.
- **Route** — another Project or conversation owns the work.
- **Pause** — a material leadership decision or unavailable authority blocks execution.

Warnings must be brief and must not interrupt routine progress unnecessarily.

## 5. Bootstrap and resume

Load only the minimum relevant context:

1. global working rules and Decision Log;
2. relevant domain or Mission README / Charter;
3. Decision Log;
4. Open Questions;
5. Work Status or latest Handoff;
6. active brief, policy or repository evidence.

Do not ask the user to repeat a decision available in authoritative records. Verify freshness before relying on operational facts.

Use the compact resume message:

```text
Context loaded: <scope and sources>
Objective: <current outcome>
Plan: <batched actions>
Blocker: <none or exact blocker>
User decision: <none or exact decision>
```

Long manual bootstrap prompts are fallback mechanisms, not the normal operating model.

## 6. Mode selection

Use `STAR_CHAT_WORK_CODEX_MODE_SELECTION.md`.

General rule:

- Chat: discussion, clarification, lightweight drafting and decisions;
- Work: sustained research, analysis, document production and cross-source synthesis;
- Codex: repository, code, tests, CI and structured GitHub implementation.

A mode label does not change authority. Durable results still require approved records.

## 7. Lifecycle and status

Conversation lifecycle:

```text
Intake → Routed → Bootstrapped → Active → Review → Waiting / Blocked → Transferred / Closed
```

Allowed statuses:

- Intake
- Routed
- Bootstrapped
- Active
- Review
- Waiting
- Blocked
- Transferred
- Closed

`Paused` may be used as a user-facing synonym for Waiting, but durable records should use the canonical values above.

A conversation is Closed only when the requested result is complete, durable records are updated, outstanding decisions are either resolved or explicitly transferred, and the Self-Review Gate passes.

## 8. Decision, memory and source rules

- Chat history and AI memory are working context only.
- Material Confirmed decisions enter the relevant append-only Decision Log.
- Current execution state enters Work Status.
- Transfer or long interruption state enters a Handoff.
- Candidate, Confirmed, Frozen, Superseded, Missing and Unverified must remain distinct.
- New decisions may not silently override active Decision IDs.
- Operational facts that may have changed must be verified from the authoritative source.
- Sensitive records must remain in approved private systems.

## 9. Handoff and closure

Create or update a Handoff when:

- work changes Project, conversation, owner or AI tool;
- the conversation is paused with material unfinished work;
- context is likely to expire;
- another team must continue execution;
- the conversation is being closed but follow-up remains elsewhere.

A receiving conversation should be able to continue from links and concise state without asking the user to reconstruct history.

Do not migrate or delete existing conversations merely to comply with this baseline.

## 10. User interruption and escalation

Continue in batches without repeated approval when work is reversible and inside confirmed scope.

Pause only when a decision:

- changes strategy, scope or governance authority;
- creates material security, compliance, financial or customer risk;
- commits costly or difficult-to-reverse architecture;
- changes an active Decision ID;
- requires a business preference between valid alternatives;
- authorizes production, rollout, migration, deletion or external commitment.

When interrupted by a new request:

- preserve current state;
- determine whether the new request belongs to the same scope;
- route or queue it explicitly;
- avoid losing the prior next action.

## 11. Failure handling

### Missing

Record the missing fact, its owner, impact and evidence required. Do not invent it.

### Stale

Verify the live source before acting. If verification is unavailable, retain the last known value with a Stale marker and date.

### Unavailable source

Use cached or secondary evidence only as Unverified. Do not claim completion, approval or current state.

### Conflicting records

Apply the authority hierarchy and Decision IDs. Escalate only if the conflict cannot be resolved through scope and provenance.

### Tool failure

Preserve the last verified state, report the failed action precisely, avoid duplicate writes and provide a safe manual path.

## 12. Validation examples

### SAIG

- Command Desk routes governance work to `⭐ STAR AI Governance`.
- SAIG loads its private repository Decision Log, Open Questions and Work Status.
- Repository migration, policy effectiveness, Wave A activation and pilot launch remain separate decisions.
- Sensitive employee and permission detail is not duplicated into public SWS records.

### Mission-001 SmartQuote

- Command Desk routes product delivery to the Mission-001 / SmartQuote professional conversation.
- Confirmed requirements are loaded from authoritative Blueprint and Decision Log rather than re-asked.
- Architecture or coding work selects Work or Codex as appropriate.
- Material requirement changes pause for product leadership; routine document and implementation work continues in batches.

## 13. Pilot usage

Pilot this baseline only in:

1. SWS-001 / SAF;
2. STAR AI Governance;
3. Mission-001 SmartQuote Foundation.

Collect evidence on routing accuracy, resume effort, repeated-user-context requests, mode mismatch warnings, handoff quality and closure accuracy before proposing freeze or broader rollout.

## 14. Enforcement

- Run the STAR Self-Review Gate after every material task or artifact.
- Update Decision Log, Open Questions, Work Status, Handoff and indexes where applicable.
- Do not freeze this baseline until pilot evidence demonstrates usability across architecture, governance and product delivery.