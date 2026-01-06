---
name: wireframe
description: Generate a text-based wireframe layout for a game UI screen
---

# UI Wireframe Generator

Create a text-based wireframe for a game UI screen.

## Process

1. Understand the screen purpose from user input
2. Identify key UI elements needed
3. Create ASCII wireframe
4. Annotate interaction patterns

## Output Format

```markdown
# Wireframe: [Screen Name]

## Purpose
[What this screen does for the player]

## Layout
```
┌────────────────────────────────────────────────────────┐
│ [Header Area]                               [Corner UI]│
├────────────────────────────────────────────────────────┤
│                                                        │
│                                                        │
│                   [Main Content]                       │
│                                                        │
│                                                        │
├────────────────────────────────────────────────────────┤
│ [Action Bar / Footer]                                  │
└────────────────────────────────────────────────────────┘
```

## Elements

| # | Element | Purpose | Interaction |
|---|---------|---------|-------------|
| 1 | [Name] | [What it shows] | [How it behaves] |
| 2 | [Name] | [What it shows] | [How it behaves] |

## Navigation
- **Enter screen from:** [Trigger]
- **Exit to:** [Possible destinations]
- **Controller shortcut:** [If applicable]

## States
[Any different states this screen can have]

## Notes
[Additional considerations]
```

## Common Screen Types

**HUD:** In-game overlay
**Inventory:** Grid of items
**Dialog:** Conversation choices
**Map:** World overview
**Settings:** Option lists
**Character:** Stats and equipment
**Shop:** Buy/sell interface

Generate appropriate wireframe based on user's description.
