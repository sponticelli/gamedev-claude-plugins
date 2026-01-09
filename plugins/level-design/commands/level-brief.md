---
name: level-brief
description: Generate a quick level design specification document
---

# Level Brief Generator

Create a concise level design specification.

## Context Gathering

Before generating the level brief, understand the context:

### Analyze Game Context
- What genre and perspective?
- What are the core mechanics?
- What's the game's pacing style?
- What's the target audience skill level?

### Understand Level Requirements
- Where does this level fit in progression?
- What mechanics should be featured?
- What's the narrative purpose?
- Are there specific set pieces needed?

### Check Existing Levels
- What patterns do existing levels follow?
- What's the established visual style?
- What duration are other levels?
- What difficulty curve exists?

### Identify Constraints
- Technical limitations?
- Asset availability?
- Time/budget constraints?
- Team experience level?

Use this context to create an appropriate level brief.

## Output Format

```markdown
# Level Brief: [Level Name]

## Quick Reference
| Attribute | Value |
|-----------|-------|
| Duration | [X-Y minutes] |
| Difficulty | [Easy/Medium/Hard] |
| Primary Mechanic | [Main skill tested] |
| Level Type | [Linear/Hub/Open] |

## Concept
[1-2 sentence elevator pitch for this level]

## Context
**Narrative:** [Why player is here]
**Before this:** [What player just did]
**After this:** [Where this leads]

## Core Experience
**The player should feel:** [Primary emotions]
**The player should learn:** [Skills/mechanics]
**Memorable moment:** [The thing players remember]

## Level Flow

### Act 1: Setup (~X%)
[Opening experience]

### Act 2: Development (~X%)
[Main gameplay]

### Act 3: Climax (~X%)
[Peak challenge]

### Act 4: Resolution (~X%)
[Cooldown and reward]

## Key Spaces
| Space | Type | Purpose |
|-------|------|---------|
| [Name] | [Arena/Corridor/Hub/etc.] | [What happens here] |

## Encounters
| Encounter | Type | Difficulty | Location |
|-----------|------|------------|----------|
| [Name] | [Combat/Puzzle/Story] | [Easy/Med/Hard] | [Which space] |

## Teaching Moments
| What's Taught | Where | How |
|---------------|-------|-----|
| [Skill] | [Location] | [Method] |

## Visual Identity
**Key colors:** [Palette]
**Mood:** [Atmosphere]
**Landmark:** [Main reference point]

## Rewards
| Reward | Type | Location |
|--------|------|----------|
| [Item] | [Required/Optional/Secret] | [Where] |

## Open Questions
[Decisions still to be made]
```

Generate based on the user's level concept and game context.
