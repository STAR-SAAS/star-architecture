# STAR Conversation Routing Matrix

| Work type | Correct Project / conversation | Default mode | Durable authority | Route or warning trigger |
|---|---|---|---|---|
| Portfolio intake, priority, routing, cross-project blocker and report-back | `STAR Command Center` / `⭐ STAR Command Desk` | Chat | Portfolio ledger plus linked professional source | Route when detailed professional work begins |
| Workspace architecture and conversation governance | `STAR OS` / `📚 STAR Architecture Framework (SAF)` | Work | `STAR-SAAS/star-architecture` | Warn if attempted in general Chat; route implementation to Codex when repository writes dominate |
| AI governance policy, standards, controls and records | `STAR OS` / `⭐ STAR AI Governance` | Work; Codex for repository changes | `STAR-SAAS/star-ai-governance` | Do not duplicate sensitive operational detail into public architecture records |
| Product and Mission requirements, blueprint and delivery planning | `STAR OS` / Mission professional conversation | Work | Mission Decision Log, Blueprint and Work Status | Route coding and repository implementation to Codex |
| Code, tests, CI, structured repository changes | Relevant delivery conversation | Codex | Repository branch, commit, PR and CI evidence | Warn when handled only in Chat or Work |
| Lightweight clarification, decision discussion or wording | Current correct professional conversation | Chat | Decision Log if material | Route if sustained research, artifact production or repository work emerges |
| Legal, compliance, finance, sales or research analysis | Corresponding professional Project and conversation | Work | Approved professional records | Route away from Command Desk and unrelated product conversations |

## Routing Gate

Before material execution:

1. identify the owning Scope;
2. state the correct Project and conversation;
3. distinguish orchestration from professional execution;
4. select Chat, Work or Codex;
5. locate the authoritative context package and Work Status;
6. proceed, warn briefly, route, or pause.

## Mismatch behavior

- **Minor mode mismatch:** warn in one sentence, then continue if safe.
- **Wrong conversation but reversible work:** identify the correct destination and preserve a handoff.
- **Wrong authority boundary:** stop professional execution and route.
- **Material leadership decision:** pause with one exact decision request.
- **Missing source:** mark Missing or Unverified; never ask the user to rebuild known history until authoritative search is exhausted.

## Pilot examples

| Prompt | Routing result |
|---|---|
| `continue M001` | Resolve Mission-001 context package, load active decisions and Work Status, continue in Mission-001 conversation; use Work or Codex according to the next task |
| `What is blocking SAIG?` | Command Desk may summarize verified portfolio status; detailed governance work routes to `⭐ STAR AI Governance` |
| `Change SmartQuote API and write tests` | Route to SmartQuote delivery / Codex; load Mission context plus repository branch and current commit |
| `Review STAR conversation governance` | SAF / Work; repository edits through Codex or GitHub workflow |
