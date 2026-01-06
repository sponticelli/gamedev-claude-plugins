---
name: pre-mortem
description: Imagine the project failed - work backwards to find what went wrong before it happens
---

# Pre-Mortem Analysis

Assume the project/decision has failed. Work backwards to identify what went wrong—before it actually happens.

## Why Pre-Mortems Work

- Overcomes optimism bias by legitimizing doubt
- Surfaces risks people are afraid to mention
- Converts "this might fail" to "this will fail because..."
- Creates actionable prevention strategies

## Process

1. Take the user's plan/project
2. Jump forward in time: it has failed
3. Generate 7-10 specific reasons why
4. Identify which are most likely and preventable
5. Create prevention actions

## Output Format

```markdown
## Pre-Mortem: [Project/Decision]

### The Setup
**Project:** [What's being attempted]
**Timeline:** [When this would be evaluated]

---

### It's [Future Date]. This Failed.

The [project] didn't work. Here's what went wrong:

#### Failure Mode 1: [Name]
**What happened:** [Specific story of how this failure occurred]
**Warning signs we missed:** [What we should have noticed]
**Likelihood:** [High/Medium/Low]
**Preventability:** [High/Medium/Low]

#### Failure Mode 2: [Name]
**What happened:** [Specific story of how this failure occurred]
**Warning signs we missed:** [What we should have noticed]
**Likelihood:** [High/Medium/Low]
**Preventability:** [High/Medium/Low]

#### Failure Mode 3: [Name]
**What happened:** [Specific story of how this failure occurred]
**Warning signs we missed:** [What we should have noticed]
**Likelihood:** [High/Medium/Low]
**Preventability:** [High/Medium/Low]

#### Failure Mode 4: [Name]
**What happened:** [Specific story of how this failure occurred]
**Warning signs we missed:** [What we should have noticed]
**Likelihood:** [High/Medium/Low]
**Preventability:** [High/Medium/Low]

#### Failure Mode 5: [Name]
**What happened:** [Specific story of how this failure occurred]
**Warning signs we missed:** [What we should have noticed]
**Likelihood:** [High/Medium/Low]
**Preventability:** [High/Medium/Low]

---

### Risk Matrix

| Failure Mode | Likelihood | Impact | Priority |
|-------------|------------|--------|----------|
| [Mode 1] | [H/M/L] | [H/M/L] | [1-5] |
| [Mode 2] | [H/M/L] | [H/M/L] | [1-5] |
| [Mode 3] | [H/M/L] | [H/M/L] | [1-5] |
| [Mode 4] | [H/M/L] | [H/M/L] | [1-5] |
| [Mode 5] | [H/M/L] | [H/M/L] | [1-5] |

---

### Prevention Plan

#### For [Top Priority Failure]
- **Early warning:** [What to monitor]
- **Prevention:** [Action to take now]
- **Contingency:** [Plan if it happens anyway]

#### For [Second Priority Failure]
- **Early warning:** [What to monitor]
- **Prevention:** [Action to take now]
- **Contingency:** [Plan if it happens anyway]

#### For [Third Priority Failure]
- **Early warning:** [What to monitor]
- **Prevention:** [Action to take now]
- **Contingency:** [Plan if it happens anyway]

---

### The Question That Matters Most
[The single most important thing to address based on this analysis]
```

## Failure Categories to Consider

- **Execution failures** - Team, timeline, quality
- **Assumption failures** - Market, customer, technology
- **External failures** - Competition, economy, regulation
- **Resource failures** - Money, people, time
- **Communication failures** - Stakeholders, team, customers

Apply to user's project/decision immediately.
