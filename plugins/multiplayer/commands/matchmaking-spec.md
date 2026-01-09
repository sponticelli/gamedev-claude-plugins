---
name: matchmaking-spec
description: Generate a matchmaking system design specification
---

# Matchmaking Specification Generator

Create a matchmaking system design document.

## Context Gathering

Before generating the matchmaking specification, understand the requirements:

### Analyze Game Mode
- What game modes exist? (1v1, team, FFA, coop)
- How many players per match?
- Are there role-based requirements? (tank, healer, etc.)
- Is cross-play supported?

### Understand Skill System
- Is there a ranking system? (MMR, ELO, tiers)
- How is skill measured?
- Are there placement matches?
- How does skill decay work?

### Check Matchmaking Priorities
- What's more important: wait time or match quality?
- Are there party/group considerations?
- Should new players be protected?
- Are there region preferences?

### Identify Constraints
- Target wait time?
- Acceptable skill range?
- Minimum player count to start?
- Backfill for in-progress matches?

Use this context to design an appropriate matchmaking system.

## Output Format

```markdown
# Matchmaking Specification: [Game Name]

## Overview
**System Type:** [Skill-based / Casual / Hybrid]
**Target Wait Time:** [Xs average, Ys max]
**Primary Goal:** [Fair matches / Fast matches / Balanced]

## Game Modes

| Mode | Players | Team Size | Skill-Based | Notes |
|------|---------|-----------|-------------|-------|
| [Mode] | [N] | [N] | [Yes/No] | [Notes] |

## Skill System

### Rating Model
**Algorithm:** [ELO / Glicko-2 / TrueSkill / Custom]
**Initial rating:** [X]
**Rating range:** [Min - Max]
**Confidence factor:** [If applicable]

### Rating Calculation
```
[Formula or description of how ratings change]
```

### Rank Tiers (if applicable)
| Tier | Rating Range | % of Players |
|------|--------------|--------------|
| [Tier] | [X - Y] | [Z%] |

### Decay Rules
[How skill decays with inactivity]

## Matchmaking Algorithm

### Queue Process
```
1. Player enters queue with [parameters]
2. [Step 2]
3. [Step 3]
4. Match formed when [conditions]
```

### Match Quality Calculation
```
[How match quality/fairness is scored]
```

### Search Expansion
| Time in Queue | Skill Range | Region Expansion |
|---------------|-------------|------------------|
| 0-30s | [Range] | [Regions] |
| 30-60s | [Range] | [Regions] |
| 60-120s | [Range] | [Regions] |
| 120s+ | [Range] | [Regions] |

## Party Handling

### Party Rules
- Max party size: [N]
- Mixed rank parties: [Allowed / Restricted / Weighted]
- Party vs solo: [Matching approach]

### Party Skill Calculation
```
[How party skill is aggregated]
```

## Special Cases

### New Player Protection
[How new players are matchmade]

### Smurfing Detection
[How smurf accounts are detected/handled]

### Leaver Handling
[What happens when players leave queue/match]

### Backfill
[Whether and how in-progress matches are filled]

## Quality Metrics

### Key Metrics
| Metric | Target | Alert Threshold |
|--------|--------|-----------------|
| Average wait time | [Xs] | [Ys] |
| Match skill delta | [X rating] | [Y rating] |
| Match completion rate | [X%] | [Y%] |
| Player satisfaction | [Measure] | [Threshold] |

### Monitoring
[How matchmaking health is monitored]

## Implementation Notes

### Required Services
[Backend services needed]

### Data Storage
[What data is stored and where]

### Scalability
[How the system scales with player count]
```

Generate based on the user's game and matchmaking requirements.
