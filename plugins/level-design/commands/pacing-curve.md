---
name: pacing-curve
description: Generate a level pacing and intensity curve
---

# Pacing Curve Generator

Create a detailed pacing analysis for a level.

## Context Gathering

Before generating the pacing curve, understand the level:

### Analyze Level Structure
- What major beats does the level have?
- How long is the level?
- What's the climax moment?
- Where are the rest points?

### Understand Pacing Goals
- What's the overall intensity target?
- When should tension peak?
- How much downtime is needed?
- What emotional journey do you want?

### Check Game Context
- What came before this level?
- What comes after?
- How does this fit the game's overall pacing?
- What player fatigue level is expected?

### Identify Key Elements
- What encounters exist?
- What story beats occur?
- What new mechanics appear?
- What rewards are given?

Use this context to design appropriate pacing.

## Output Format

```markdown
# Pacing Analysis: [Level Name]

## Overview
**Total Duration:** [X-Y minutes]
**Overall Intensity:** [Low / Medium / High]
**Emotional Arc:** [e.g., Tension → Release → Climax → Resolution]

## Intensity Graph

```
HIGH   │           ╱╲
       │          ╱  ╲         ╱╲
MEDIUM │    ╱╲   ╱    ╲   ╱╲  ╱  ╲
       │   ╱  ╲ ╱      ╲ ╱  ╲╱    ╲
LOW    │──╱    ╳        ╳          ╲──
       │
       └─────────────────────────────────
        0%   25%   50%   75%   100%
        │     │     │     │     │
     Entry  Rising Peak  Falling Exit
```

## Beat-by-Beat Breakdown

### Opening (0-X%)
**Duration:** [Minutes]
**Intensity:** [Level]
**Purpose:** [What this section accomplishes]

| Beat | Type | Intensity | Duration | Notes |
|------|------|-----------|----------|-------|
| [Beat] | [Combat/Puzzle/Story/Explore] | [1-10] | [Time] | [Details] |

### Rising Action (X-Y%)
**Duration:** [Minutes]
**Intensity:** [Level]
**Purpose:** [What this section accomplishes]

| Beat | Type | Intensity | Duration | Notes |
|------|------|-----------|----------|-------|
| [Beat] | [Type] | [1-10] | [Time] | [Details] |

### Climax (Y-Z%)
**Duration:** [Minutes]
**Intensity:** [Level]
**Purpose:** [What this section accomplishes]

| Beat | Type | Intensity | Duration | Notes |
|------|------|-----------|----------|-------|
| [Beat] | [Type] | [1-10] | [Time] | [Details] |

### Resolution (Z-100%)
**Duration:** [Minutes]
**Intensity:** [Level]
**Purpose:** [What this section accomplishes]

| Beat | Type | Intensity | Duration | Notes |
|------|------|-----------|----------|-------|
| [Beat] | [Type] | [1-10] | [Time] | [Details] |

## Intensity Factors

### What Raises Intensity
| Factor | Where Used | Intensity Boost |
|--------|------------|-----------------|
| [Factor] | [Beat(s)] | [+X] |

### What Lowers Intensity
| Factor | Where Used | Intensity Drop |
|--------|------------|----------------|
| [Factor] | [Beat(s)] | [-X] |

## Rest Points

| Location | Duration | Purpose |
|----------|----------|---------|
| [Where] | [How long] | [Why rest here] |

## Emotion Journey

```
EMOTION GRAPH:

Wonder  │        *
        │       /
Hope    │      *
        │     /
Neutral │----*
        │     \
Tension │      *
        │       \    *
Fear    │        *--/
        │
        └────────────────
          Start      End
```

## Pacing Issues & Solutions

| Potential Issue | Location | Solution |
|-----------------|----------|----------|
| [Issue] | [Where] | [How to fix] |

## Comparison to Game Average

| Metric | This Level | Game Average | Notes |
|--------|-----------|--------------|-------|
| Peak intensity | [X/10] | [Y/10] | [Context] |
| Rest frequency | [Every X min] | [Every Y min] | [Context] |
| Combat % | [X%] | [Y%] | [Context] |
```

Generate based on the user's level and pacing goals.
