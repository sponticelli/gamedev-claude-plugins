---
name: algorithm-eval
description: Evaluate which PCG algorithm fits specific needs
---

# Algorithm Evaluation Generator

Evaluate and recommend PCG algorithms for a specific use case.

## Context Gathering

Before evaluating algorithms, understand the requirements:

### Analyze Content Type
- What exactly is being generated?
- What properties must the output have?
- What's the expected variety?
- What's the quality expectation?

### Understand Constraints
- What performance budget exists?
- What memory is available?
- What's the team's algorithm experience?
- What libraries/frameworks are available?

### Check Integration
- How does this fit with other systems?
- What's the input format?
- What's the output format?
- What post-processing is expected?

### Identify Priorities
- Speed or quality?
- Variety or consistency?
- Control or emergence?
- Simple or powerful?

Use this context to evaluate and recommend algorithms.

## Output Format

```markdown
# Algorithm Evaluation: [Use Case]

## Requirements Summary

### Content
**Type:** [What's generated]
**Scale:** [How much/how big]
**Quality:** [Expectations]

### Technical
**Time budget:** [ms]
**Memory budget:** [MB]
**Platform:** [Targets]

### Team
**Experience level:** [Novice/Intermediate/Expert]
**Libraries available:** [Options]

## Candidate Algorithms

### Option 1: [Algorithm Name]

**Overview:**
[How the algorithm works]

**Pros:**
- [Advantage 1]
- [Advantage 2]
- [Advantage 3]

**Cons:**
- [Disadvantage 1]
- [Disadvantage 2]

**Performance:**
- Time complexity: [O(?)]
- Memory: [Usage pattern]
- Parallelizable: [Yes/No]

**Implementation:**
- Difficulty: [Easy/Medium/Hard]
- Lines of code: [Estimate]
- Libraries: [Available options]

**Fit score:** [1-10]

---

### Option 2: [Algorithm Name]
[Same structure]

---

### Option 3: [Algorithm Name]
[Same structure]

## Comparison Matrix

| Criteria | Weight | [Algo 1] | [Algo 2] | [Algo 3] |
|----------|--------|----------|----------|----------|
| Speed | [W] | [Score] | [Score] | [Score] |
| Quality | [W] | [Score] | [Score] | [Score] |
| Control | [W] | [Score] | [Score] | [Score] |
| Simplicity | [W] | [Score] | [Score] | [Score] |
| **Weighted** | | **[Total]** | **[Total]** | **[Total]** |

## Recommendation

### Primary: [Algorithm Name]

**Why:**
[Justification for this choice]

**When to reconsider:**
[Conditions that would change the recommendation]

### Fallback: [Algorithm Name]

**When to use instead:**
[When the fallback is better]

## Implementation Approach

### Steps
1. [Implementation step 1]
2. [Implementation step 2]
3. [Implementation step 3]

### Key Parameters
| Parameter | Purpose | Tuning Notes |
|-----------|---------|--------------|
| [Param] | [What it does] | [How to tune] |

### Pitfalls to Avoid
- [Common mistake 1]
- [Common mistake 2]

## Resources

### References
- [Paper/tutorial 1]
- [Paper/tutorial 2]

### Example Implementations
- [Code example 1]
- [Code example 2]
```

Generate based on the user's use case and requirements.
