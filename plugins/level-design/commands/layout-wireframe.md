---
name: layout-wireframe
description: Generate a text-based level layout description
---

# Layout Wireframe Generator

Create a textual level layout description.

## Context Gathering

Before generating the layout, understand the requirements:

### Analyze Space Needs
- What activities happen in this level?
- What's the flow (linear, hub, open)?
- How many major spaces are needed?
- What connections between spaces?

### Understand Technical Limits
- What's the maximum size?
- Are there streaming/loading considerations?
- What perspective (2D, 3D, isometric)?
- Platform performance limits?

### Check Design Requirements
- Encounter spaces needed?
- Navigation landmarks needed?
- Backtracking requirements?
- Secret areas planned?

### Identify Style
- Interior, exterior, or mixed?
- Vertical gameplay needed?
- Water/hazard areas?
- Themed zones?

Use this context to create appropriate layout.

## Output Format

```markdown
# Level Layout: [Level Name]

## Overview
**Dimensions:** [Approximate X × Y × Z]
**Flow Type:** [Linear / Hub / Open / Branching]
**Primary Direction:** [North-South / East-West / Vertical / Mixed]
**Estimated Traversal:** [X minutes without combat]

## ASCII Layout

### Top-Down View
```
LEGEND:
[E] = Entry       [X] = Exit
[A] = Arena       [C] = Corridor
[H] = Hub         [S] = Safe Room
[P] = Puzzle      [V] = Vista Point
[#] = Wall/Solid  [ ] = Open Space
[/] = Slope/Ramp  [|] = Vertical Connection

LAYOUT:
┌─────────────────────────────────────┐
│                                     │
│  [E]──[C]──[A]──[C]──[H]           │
│                     │   │           │
│                  [P]┘   └──[A]      │
│                             │       │
│                          [V]┘       │
│                             │       │
│                          [S]──[X]   │
│                                     │
└─────────────────────────────────────┘
```

### Side View (if vertical)
```
Level 3: [Vista]
         |
Level 2: [Arena]──[Corridor]
              |
Level 1: [Entry]──[Hub]
```

## Space Descriptions

### [Space Name] (Type: [Arena/Corridor/Hub/etc.])
**Position:** [Relative location in layout]
**Size:** [Small/Medium/Large]
**Connections:** [What it links to]
**Purpose:** [Why this space exists]
**Key features:** [Notable elements]

[Repeat for each major space]

## Flow Analysis

### Critical Path
```
[Entry] → [Space A] → [Space B] → [Space C] → [Exit]
```

### Optional Paths
```
[Hub] → [Secret Area] (requires: [condition])
[Arena B] → [Hidden Room] (requires: [condition])
```

### Backtracking
[When and why player returns to previous spaces]

## Vertical Structure
| Level | Height | Contents |
|-------|--------|----------|
| [N] | [Meters] | [What's here] |

## Sightlines

### Long Views
| From | To | Purpose |
|------|-----|---------|
| [Space] | [Target] | [Why this view exists] |

### Key Reveals
[What's revealed when, for dramatic effect]

## Navigation Aids

### Landmarks
| Landmark | Visible From | Purpose |
|----------|--------------|---------|
| [Object] | [Spaces] | [How it helps navigation] |

### Wayfinding
[How players know where to go]

## Technical Notes
[Streaming boundaries, performance considerations, etc.]
```

Generate based on the user's level requirements.
