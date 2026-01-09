---
name: constraint-rules
description: Generate content generation constraints and validation rules
---

# Constraint Rules Generator

Create constraint definitions for procedural content.

## Context Gathering

Before generating constraints, understand the requirements:

### Analyze Content Type
- What is being generated?
- What makes it valid?
- What makes it good?
- What must never happen?

### Understand Gameplay
- What gameplay must the content support?
- What player expectations exist?
- What would break the experience?
- What variety is needed?

### Check Technical Limits
- What validation is computationally feasible?
- How fast must validation be?
- What repair strategies are available?
- How are failures handled?

### Identify Priorities
- Which constraints are non-negotiable?
- Which are preferences?
- How should conflicts be resolved?
- What quality tradeoffs exist?

Use this context to create constraint rules.

## Output Format

```markdown
# Constraint Rules: [Content Type]

## Overview
**Content:** [What's constrained]
**Philosophy:** [Strict/Balanced/Loose]
**Validation timing:** [Pre/During/Post generation]

## Hard Constraints (Must Pass)

### HC1: [Constraint Name]
**Rule:** [What must be true]
**Rationale:** [Why this matters]
**Formal definition:**
```
[Logic or pseudocode]
```
**Validation:**
```
[How to check]
```
**Repair strategy:**
[How to fix violations]

**Priority:** P0 (Critical)

---

### HC2: [Constraint Name]
[Same structure]

---

[Continue for all hard constraints]

## Soft Constraints (Should Pass)

### SC1: [Constraint Name]
**Goal:** [What should be true]
**Rationale:** [Why this improves quality]
**Weight:** [1-10, importance relative to other soft constraints]
**Scoring:**
```
[How to measure compliance, 0-1]
```
**Acceptable threshold:** [Minimum passing score]

---

### SC2: [Constraint Name]
[Same structure]

---

[Continue for all soft constraints]

## Quality Preferences

### QP1: [Preference Name]
**Preference:** [What's better]
**Measure:** [How to score]
**Weight:** [Importance]

---

[Continue for all preferences]

## Constraint Interactions

### Conflicts
| Constraint A | Constraint B | Conflict | Resolution |
|--------------|--------------|----------|------------|
| [Name] | [Name] | [What conflicts] | [Priority] |

### Dependencies
| Constraint | Depends On | Order |
|------------|------------|-------|
| [Name] | [Name] | [Check order] |

## Validation Pipeline

### Stage 1: [Pre-Generation]
**Constraints checked:**
- [Constraint 1]
- [Constraint 2]

**On failure:** [Action]

### Stage 2: [During Generation]
**Constraints checked:**
- [Constraint 1]
- [Constraint 2]

**On failure:** [Action]

### Stage 3: [Post-Generation]
**Constraints checked:**
- [Constraint 1]
- [Constraint 2]

**On failure:** [Action]

## Composite Quality Score

**Formula:**
```
quality = (
    hard_pass ×
    (w1×soft1 + w2×soft2 + ... + wn×softn) ×
    (1 + bonus_factors)
)
```

**Thresholds:**
| Level | Score | Action |
|-------|-------|--------|
| Reject | < X | Regenerate |
| Accept | X - Y | Use as-is |
| Great | > Y | Mark as high quality |

## Debug Visualization

### What to Show
- [Visualization 1]
- [Visualization 2]

### Constraint Overlays
[How to display constraint states]
```

Generate based on the user's content and constraint requirements.
