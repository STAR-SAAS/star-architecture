# STAR Conversation Routing Matrix

| Work type | Correct Project / conversation | Recommended available mode | Durable authority | Route or warning trigger |
|---|---|---|---|---|
| Portfolio intake, priority, routing, cross-project blocker and report-back | `STAR Command Center` / `⭐ STAR Command Desk` | Chat | Portfolio ledger plus linked professional source | Route when detailed professional work begins |
| Workspace architecture and conversation governance | `STAR OS` / `📚 STAR Architecture Framework (SAF)` | Work; GitHub/Codex workflow for repository edits | `STAR-SAAS/star-architecture` | Warn if attempted in general Chat; route implementation when repository work dominates |
| AI governance policy, standards, controls and records | `STAR OS` / `⭐ STAR AI Governance` | Work; GitHub/Codex workflow for repository edits | `STAR-SAAS/star-ai-governance` | Keep sensitive operational detail in approved private sources |
| Product and Mission requirements, blueprint and delivery planning | `STAR OS` / Mission professional conversation | Work | Mission Decision Log, Blueprint and Work Status | Route coding and implementation to available Codex/GitHub workflow |
| Code, tests, CI, structured repository changes | Relevant delivery conversation | Codex or available repository workflow | Branch, commit, PR and CI evidence | Warn when handled only in lightweight Chat |
| Lightweight clarification, decision discussion or wording | Current correct professional conversation | Chat | Decision Log if material | Route if sustained research, artifact production or repository work emerges |
| Legal, compliance, finance, sales or research analysis | Corresponding professional Project and conversation | Work | Approved professional records | Route away from Command Desk and unrelated product conversations |

## Routing Gate

Before material execution:

1. identify the owning Scope;
2. state the correct Project and conversation;
3. distinguish orchestration from professional execution;
4. recommend or use the most suitable available mode;
5. locate the authoritative Context Package and Work Status;
6. proceed, warn briefly, route, or pause.

## Lifecycle-aware routing

Primary path:

```text
Intake → Routed → Bootstrapped → Active → Review → Closed
```

- Waiting and Blocked are interrupt states available from Routed, Bootstrapped, Active or Review.
- Record `prior_state` before entering either interrupt state.
- Waiting returns to `prior_state` when awaited input arrives.
- Blocked returns to `prior_state` after the blocker is resolved.
- Transfer records the sender as Transferred and starts the receiver at Bootstrapped through a Handoff.
- Closed is not silently reopened; new work uses a new Activity / Contract unless a governed Reopened rule is later approved.

## Mismatch behavior

- **Minor mode mismatch:** warn in one sentence, then continue if safe.
- **Direct mode transfer unavailable:** preserve the Contract and create a Handoff.
- **Wrong conversation but reversible work:** identify the correct destination and preserve state.
- **Wrong authority boundary:** stop professional execution and route.
- **Material leadership decision:** pause with one exact decision request.
- **Missing source:** mark Missing or Unverified; search authoritative sources before asking the user to reconstruct history.

## Pilot examples

| Prompt | Routing result |
|---|---|
| `continue M001` | Resolve the authoritative alias and M001 package, reuse the Contract, load changed required payload only, and recommend Work or Codex; conceptually validated, operationally Unverified |
| `What is blocking SAIG?` | Command Desk may summarize verified coordination status; detailed governance work routes to `⭐ STAR AI Governance` and private sources |
| `Change SmartQuote API and write tests` | Route to SmartQuote delivery and available Codex/GitHub workflow; load Mission context plus task-relevant repository evidence |
| `Review STAR conversation governance` | SAF / Work; repository edits through an available GitHub/Codex workflow |
