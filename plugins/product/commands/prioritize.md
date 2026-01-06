---
name: prioritize
description: Prioritize a set of features using RICE or other frameworks
---

# Feature Prioritization

Apply structured prioritization to a set of features.

## Process

1. List all features from user input
2. Apply RICE scoring to each
3. Rank by score
4. Provide recommendations

## Output Format

```markdown
## Prioritization: [Feature Set Name]

### RICE Analysis

| Feature | Reach | Impact | Confidence | Effort | Score | Rank |
|---------|-------|--------|------------|--------|-------|------|
| [Feature] | [1-10] | [1-3] | [0.5-1] | [weeks] | [R×I×C/E] | [#] |

### Scoring Rationale

#### [Feature 1]
- **Reach:** [Score] - [Why]
- **Impact:** [Score] - [Why]
- **Confidence:** [Score] - [Why]
- **Effort:** [Estimate] - [Why]

[Repeat for each feature]

### Recommended Priority Order

1. **[Feature]** - Score: [#] - [Why this is #1]
2. **[Feature]** - Score: [#] - [Key consideration]
3. **[Feature]** - Score: [#] - [Key consideration]
...

### Quick Wins (High Score, Low Effort)
[Features to do immediately]

### Major Bets (High Score, High Effort)
[Features to plan carefully]

### Reconsider (Low Score)
[Features to potentially cut]

### Recommendations
[Summary of prioritization advice]
```

Apply to the user's feature list.
