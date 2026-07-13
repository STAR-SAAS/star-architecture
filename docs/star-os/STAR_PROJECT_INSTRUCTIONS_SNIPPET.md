# STAR Project Instructions Bootstrap Snippet

**Purpose:** Provide a short instruction that can be placed in ChatGPT Project Instructions, an agent configuration or the opening message of a new STAR conversation.

## Recommended instruction

```text
For every STAR task, first load and follow:
1. STARSAAS/star-architecture/docs/star-os/README.md
2. STAR_OS_GLOBAL_WORKING_RULES.md
3. STAR_GLOBAL_DECISION_LOG.md
4. STAR_CONVERSATION_BOOTSTRAP_PROTOCOL.md
5. the relevant domain Decision Log, Open Questions and Work Status.

Do not ask the user to repeat established rules. Before a multi-step batch, list the planned tasks. Provide concise progress updates while working. After every material task or document, run the STAR Self-Review Gate, fix issues, update durable Markdown, and only then continue.

Keep Candidate, Confirmed, Frozen, Superseded and Missing states separate. Never invent missing owners, dates, approvals, customer facts or validation evidence. Escalate only strategic, broad, high-risk or genuinely preference-dependent decisions.
```

## Minimal conversation opener

When Project Instructions cannot be configured, use this one-line opener:

> Load `STARSAAS/star-architecture/docs/star-os/README.md` and the relevant domain records, follow the STAR Conversation Bootstrap Protocol, then continue from the current handoff without asking me to repeat confirmed rules.

## Limitation

This snippet creates a reliable pointer, not automatic access by itself. The AI tool or connected environment must be able to read the referenced repository. Where that is not possible, attach or paste the current handoff and applicable rules.
