---
name: animation-spec
description: Generate an animation system and state machine design
---

# Animation Specification Generator

Create an animation system design document.

## Context Gathering

Before generating the animation spec, understand the requirements:

### Analyze Character Needs
- What type of character? (Player, NPC, creature)
- What locomotion modes? (Walk, run, swim, fly)
- What actions are needed? (Combat, interact, emote)
- How responsive must it feel?

### Understand Technical Context
- What engine/animation system?
- What skeleton structure exists?
- What's the performance budget?
- What platforms are targeted?

### Check Existing Animation
- Are there existing animations to work with?
- What animation style is established?
- What's the current state machine (if any)?
- What problems need solving?

### Identify Requirements
- Must-have animations?
- Nice-to-have animations?
- IK requirements?
- Procedural animation needs?

Use this context to design appropriate animation system.

## Output Format

```markdown
# Animation System Specification: [Character/Feature]

## Overview
**Character:** [Who this is for]
**Locomotion:** [Root motion / In-place]
**Responsiveness:** [Required input latency]
**Complexity:** [State count estimate]

## Skeleton

### Hierarchy
```
[Bone hierarchy diagram]
```

### Bone Count
| LOD | Bone Count | Use Case |
|-----|------------|----------|
| Full | [N] | Close-up |
| LOD1 | [N] | Medium |
| LOD2 | [N] | Far |

## State Machine

### Overview Diagram
```
[State machine diagram]
```

### States

#### [State Name]
**Purpose:** [What this state does]
**Animation:** [What plays]
**Entry:** [How to enter]
**Exit:** [How to exit]
**Duration:** [Loop/time/event]

[Repeat for each state]

### Transitions
| From | To | Condition | Duration | Interruptible |
|------|-----|-----------|----------|---------------|
| [State] | [State] | [Condition] | [Time] | [Yes/No] |

## Blend Trees

### [Blend Tree Name]
**Type:** [1D/2D/Direct]
**Parameter(s):** [What drives it]
**Clips:**
| Position | Animation | Notes |
|----------|-----------|-------|
| [Value(s)] | [Clip] | [Details] |

## Layers

| Layer | Purpose | Blend Mode | Mask |
|-------|---------|------------|------|
| [N] | [What it does] | [Override/Additive] | [Body parts] |

## IK Requirements

### [IK System]
**Type:** [Foot/Hand/Look/Aim]
**When active:** [Conditions]
**Targets:** [What's controlled]
**Blend:** [How it fades in/out]

## Animation List

### Required
| Animation | Length | Priority |
|-----------|--------|----------|
| [Name] | [Seconds] | [P0/P1/P2] |

### Nice to Have
| Animation | Length | Notes |
|-----------|--------|-------|
| [Name] | [Seconds] | [Why wanted] |

## Performance Budget
**Max evaluated nodes:** [N]
**Max active layers:** [N]
**Max blend tree depth:** [N]

## Implementation Notes
[Technical considerations, dependencies, risks]
```

Generate based on the user's character and animation needs.
