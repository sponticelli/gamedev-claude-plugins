---
name: bias-check
description: Quick cognitive bias scan - identify biases that might be affecting a decision or belief
---

# Quick Bias Check

Rapidly scan a decision or belief for common cognitive biases.

## Process

1. Understand the decision/belief from user input
2. Scan for top 5 most likely biases
3. For each, explain how it might be affecting thinking
4. Provide one debiasing question per bias

## Output Format

```markdown
## Bias Check: [Decision/Belief]

### Quick Assessment
[One sentence on overall bias risk: Low/Medium/High]

### Likely Biases

#### 1. [Bias Name]
**How it might be showing up:** [Specific manifestation]
**Debiasing question:** [Question to counteract it]

#### 2. [Bias Name]
**How it might be showing up:** [Specific manifestation]
**Debiasing question:** [Question to counteract it]

#### 3. [Bias Name]
**How it might be showing up:** [Specific manifestation]
**Debiasing question:** [Question to counteract it]

#### 4. [Bias Name]
**How it might be showing up:** [Specific manifestation]
**Debiasing question:** [Question to counteract it]

#### 5. [Bias Name]
**How it might be showing up:** [Specific manifestation]
**Debiasing question:** [Question to counteract it]

### The One Thing to Do
[Single most important debiasing action for this situation]
```

## Common Bias Patterns by Situation

**When continuing a project:**
- Sunk cost fallacy, Commitment escalation, Status quo bias

**When starting something new:**
- Optimism bias, Planning fallacy, Overconfidence

**When evaluating an idea:**
- Confirmation bias, Anchoring, Halo effect

**When in a group:**
- Groupthink, Authority bias, Bandwagon effect

**When analyzing past events:**
- Hindsight bias, Survivorship bias, Attribution errors

Apply to user's decision immediately.
