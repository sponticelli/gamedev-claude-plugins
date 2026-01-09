---
name: encounter-spec
description: Generate a single encounter design specification
---

# Encounter Specification Generator

Create a detailed design for a single encounter.

## Context Gathering

Before generating the encounter spec, understand the context:

### Analyze Encounter Purpose
- Is this combat, puzzle, or hybrid?
- What skill/mechanic is being tested?
- Is this teaching or testing?
- What's the dramatic purpose?

### Understand Placement
- Where in the level does this occur?
- What comes before and after?
- What resources does player have?
- What's the current intensity?

### Check Game Systems
- What enemies/mechanics are available?
- What difficulty settings exist?
- What are player capabilities at this point?
- Any special rules or constraints?

### Identify Goals
- What should player learn?
- What should player feel?
- How long should it take?
- What's the reward?

Use this context to design appropriate encounter.

## Output Format

```markdown
# Encounter Spec: [Encounter Name]

## Quick Reference
| Attribute | Value |
|-----------|-------|
| Type | [Combat / Puzzle / Hybrid] |
| Difficulty | [Easy / Medium / Hard / Boss] |
| Duration | [X-Y seconds/minutes] |
| Location | [Level and space] |

## Purpose
**Gameplay purpose:** [What skill is tested]
**Narrative purpose:** [What story is told]
**Pacing purpose:** [Why here in the level]

## Space

### Layout
```
[ASCII diagram of encounter space]
```

### Key Features
| Feature | Position | Function |
|---------|----------|----------|
| [Feature] | [Where] | [What it does] |

## Combat Details (if applicable)

### Enemy Composition
| Enemy | Count | Role | Behavior |
|-------|-------|------|----------|
| [Type] | [N] | [Role] | [What they do] |

### Spawn Points
[Where enemies appear]

### Waves (if applicable)
| Wave | Trigger | Composition |
|------|---------|-------------|
| [N] | [What starts it] | [Enemies] |

### AI Notes
[Special behaviors, coordination, etc.]

## Puzzle Details (if applicable)

### Mechanics Used
[What abilities/tools needed]

### Elements
| Element | Type | Interaction |
|---------|------|-------------|
| [Object] | [Interactive/Hazard/Clue] | [What it does] |

### Solution
**Intended solution:**
1. [Step 1]
2. [Step 2]
3. [Step 3]

**Alternative solutions (if any):**
[Other valid approaches]

### Hints
[What points players toward solution]

## Difficulty Scaling

### Base Difficulty
[Standard challenge level]

### Easy Mode Adjustments
- [Change 1]
- [Change 2]

### Hard Mode Adjustments
- [Change 1]
- [Change 2]

## Player Experience

### Entry
**What player sees:** [First impression]
**What player hears:** [Audio cues]
**Initial emotion:** [How they should feel]

### During
**Core loop:** [What player does repeatedly]
**Challenge peak:** [Hardest moment]
**Key decisions:** [Meaningful choices]

### Exit
**Victory feel:** [Emotion on success]
**Reward:** [What player gets]
**Transition:** [How it leads to next area]

## Failure Handling

### Fail Conditions
[What counts as failure]

### Fail State
[What happens on failure]

### Recovery
[How player can try again]

## Edge Cases

| Scenario | Handling |
|----------|----------|
| [Edge case] | [What happens] |

## Implementation Notes

### Triggers
| Trigger | Condition | Action |
|---------|-----------|--------|
| [Name] | [When] | [What happens] |

### Required Assets
| Asset | Type | Notes |
|-------|------|-------|
| [Asset] | [Enemy/Prop/Sound/etc.] | [Requirements] |

### Testing Checklist
- [ ] Beatable on all difficulty settings
- [ ] No exploit/skip opportunities (unless intended)
- [ ] Clear victory/failure communication
- [ ] Rewards given correctly
- [ ] No soft-lock possibilities
```

Generate based on the user's encounter concept and game context.
