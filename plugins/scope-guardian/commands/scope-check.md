---
name: scope-check
description: Quick check if a feature aligns with design pillars - get an instant yes/no/maybe verdict
---

# Quick Scope Check

Rapidly evaluate whether a proposed feature belongs in the project.

## Process

1. Identify the feature from user input
2. Identify design pillars (ask if not provided)
3. Run pillar alignment check
4. Assess hidden costs
5. Deliver verdict

## Output Format

```markdown
## Scope Check: [Feature Name]

### Pillar Alignment
| Pillar | Supports? | Reasoning |
|--------|-----------|-----------|
| [Pillar 1] | Yes/No/Partial | [One sentence] |
| [Pillar 2] | Yes/No/Partial | [One sentence] |
| [Pillar 3] | Yes/No/Partial | [One sentence] |

**Alignment:** [X/Y] pillars

### Quick Cost Check
- **Dev effort:** [Low/Med/High]
- **Hidden costs:** [List 2-3 biggest]
- **Maintenance burden:** [Low/Med/High]

### Verdict: [APPROVE / DEFER / REDUCE / REJECT]

**Reasoning:** [2-3 sentences explaining the verdict]

### If Approved
[Any caveats or conditions]

### If Rejected/Deferred
[Alternative suggestion or smaller version]
```

## Verdict Criteria

- **APPROVE:** Aligns with 2+ pillars, reasonable cost, clear value
- **DEFER:** Good idea but wrong timing - add to post-launch list
- **REDUCE:** Core concept is sound but scope is too big - suggest smaller version
- **REJECT:** Doesn't align with pillars or cost far exceeds value

## Quick Questions (if context is missing)

If the user hasn't provided pillars, ask:
"What are your 3-5 design pillars? (The core principles that define what makes your game special)"
