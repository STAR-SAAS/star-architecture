# [CTX-000] AI Context Package

**Purpose:** Give an AI only the current, relevant and authorized context needed for one bounded task.

| Field | Value |
|---|---|
| **Task / Work Item** |  |
| **AI work level** | A0 / A1 / A2 / A3 / A4 |
| **Accountable human** |  |
| **Human reviewer / approver** |  |
| **Created** | YYYY-MM-DD HH:MM TZ |
| **Expires / review trigger** |  |
| **Status** | Draft / Authorized / Used / Expired / Revoked |

## 1. Required outcome

- **Requested result:**
- **Completion evidence:**
- **Why this work matters:**
- **Related Mission / decision:**

## 2. Scope

- **Products / repositories / paths:**
- **Environment / data boundary:**
- **Time boundary:**
- **Explicitly out of scope:**

## 3. Authoritative sources

| Source | Link / ID | Version / commit / timestamp | Owner / status | Why relevant |
|---|---|---|---|---|
|  |  |  |  |  |

Only listed or explicitly linked sources are authoritative for this task. Chat summaries and AI output are working input unless reviewed and recorded in the correct source.

## 4. Current decisions and constraints

- **Confirmed decisions:**
- **Applicable standards / policies:**
- **Known assumptions:**
- **Open questions:**
- **Conflicts or uncertainty:**

## 5. Authorization

### Allowed actions

- 

### Prohibited actions

- 

### Allowed tools and systems

- 

### Required stop / escalation conditions

- conflicting authoritative sources;
- missing permission or required context;
- action exceeds scope or risk level;
- required check fails;
- secret, restricted or customer data may be exposed;
- a confirmed decision would be violated.

## 6. Validation and review

- **Automated checks:**
- **Human review:**
- **Independent approval if required:**
- **Rollback / recovery:**
- **Operational or customer observation:**

## 7. Execution record

- **Actions taken:**
- **Outputs / commits / artifacts:**
- **Checks passed / failed:**
- **Uncertainty remaining:**
- **Escalation or follow-up:**

## Authoring rules

1. Keep the package specific to one task or tightly bounded work batch.
2. Use source links, versions and timestamps; do not paste unnecessary copies.
3. Grant the minimum actions and data needed.
4. Expire the package when the task, source state or authorization changes materially.
5. AI output does not become authoritative merely because it used an authorized context package.
