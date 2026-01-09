---
name: difficulty-curve
description: Generate a dynamic difficulty system design
---

# Difficulty Curve Generator

Create a dynamic difficulty adjustment system design.

## Context Gathering

Before generating the difficulty curve, understand the game:

### Analyze Game Type
- What genre is the game?
- What creates challenge? (Combat, puzzles, platforming)
- What's the skill ceiling?
- How long is the game?

### Understand Target Audience
- Who is this game for?
- What skill range do you expect?
- Is accessibility a priority?
- Competitive or casual focus?

### Check Existing Balance
- What difficulty options exist?
- What's been tuned already?
- What do playtesters struggle with?
- What feels too easy?

### Identify Adjustable Elements
- What can change to affect difficulty?
- What should NOT change?
- What's visible vs invisible?
- What's per-attempt vs per-session?

Use this context to design appropriate difficulty system.

## Output Format

```markdown
# Difficulty System: [Game Name]

## Overview
**Approach:** [Fixed/Adaptive/Hybrid]
**Player control:** [Full/Partial/None]
**Adjustment speed:** [Aggressive/Moderate/Gentle]

## Difficulty Levels (if explicit)

| Level | Target Audience | Key Differences |
|-------|-----------------|-----------------|
| [Easy] | [Who] | [What changes] |
| [Normal] | [Who] | [Baseline] |
| [Hard] | [Who] | [What changes] |

## Player Skill Tracking

### Metrics
| Metric | Weight | Collection |
|--------|--------|------------|
| [Metric] | [Importance] | [How measured] |

### Skill Estimation
**Formula:** [How skill is calculated]
**Window:** [How much history is used]
**Smoothing:** [How spikes are handled]

### Performance Bands
| Band | Skill Range | Response |
|------|-------------|----------|
| [Struggling] | [0-X] | [Easier] |
| [Appropriate] | [X-Y] | [Maintain] |
| [Dominating] | [Y-100] | [Harder] |

## Adjustment Mechanisms

### Enemy Adjustments
| Element | Easy | Normal | Hard | Adaptive Range |
|---------|------|--------|------|----------------|
| Health | [%] | 100% | [%] | [Min-Max %] |
| Damage | [%] | 100% | [%] | [Min-Max %] |
| Speed | [%] | 100% | [%] | [Min-Max %] |
| Count | [%] | 100% | [%] | [Min-Max %] |

### Player Adjustments
| Element | Easy | Normal | Hard | Adaptive Range |
|---------|------|--------|------|----------------|
| Health | [%] | 100% | [%] | [Min-Max %] |
| Damage | [%] | 100% | [%] | [Min-Max %] |
| Resources | [%] | 100% | [%] | [Min-Max %] |

### System Adjustments
| Element | Effect | When Applied |
|---------|--------|--------------|
| [Element] | [What changes] | [Trigger] |

## Target Experience

### Flow Metrics
| Metric | Target | Too Low | Too High |
|--------|--------|---------|----------|
| Death rate | [X/hr] | Increase diff | Decrease diff |
| Time per encounter | [Xm] | [Action] | [Action] |
| Resource usage | [X%] | [Action] | [Action] |

### Pacing Curve
```
Challenge
    ↑
    │      ╱╲      ╱╲
    │    ╱    ╲  ╱    ╲
    │  ╱        ╲        ╲
    │╱                     ╲
    └─────────────────────────→
      Tutorial  Mid-game  End
```

## Special Rules

### Mercy Mechanics
| Trigger | Action | Reset |
|---------|--------|-------|
| [X deaths on boss] | [Reduce boss health] | [After victory] |

### Skill Gate Protection
[What prevents trivializing key challenges]

### Anti-Exploit
[What prevents gaming the system]

## Transparency

### Shown to Player
[What player sees about difficulty]

### Hidden from Player
[What adjusts invisibly]

## Implementation

### When to Adjust
**Check frequency:** [Every X seconds/On death/etc.]
**Apply timing:** [Immediately/Next encounter/etc.]

### Bounds
**Floor:** [Minimum difficulty regardless of struggle]
**Ceiling:** [Maximum difficulty regardless of skill]

## Verification
**Test scenarios:** [How to verify it works]
**Telemetry:** [What to track]
```

Generate based on the user's game and difficulty needs.
