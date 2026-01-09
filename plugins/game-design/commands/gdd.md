---
name: gdd
description: Generate a Game Design Document outline with proper structure and sections tailored to the game concept
---

# Game Design Document Generator

Create a structured GDD outline based on the user's game concept.

## Context Gathering

Before generating the GDD, understand the project context:

### Check for Existing Documentation
- Look for files matching: `*gdd*`, `*design*`, `*spec*`, `README*`
- Read any existing documentation to understand current state
- Note what's already defined vs. what needs to be created

### Identify Project Type
- **Unity:** Look for `.meta` files, `Assets/` folder, `ProjectSettings/`
- **Godot:** Look for `project.godot`, `*.tscn`, `*.gd` files
- **Unreal:** Look for `.uproject` files, `Content/` folder
- **Custom/Other:** Look for `package.json`, `Cargo.toml`, build files

### Understand Scope
- Check git history to gauge project maturity
- Count source files to estimate project size
- Look for existing assets to gauge production stage
- Review any existing design notes or concepts

Use this context to:
- Reference existing decisions rather than re-inventing them
- Match the GDD scope to the project stage
- Incorporate existing terminology and naming conventions
- Identify what sections need the most attention

## Process

1. Understand the game concept from user input
2. Identify the game's scope (prototype/vertical slice/full production)
3. Generate appropriate sections
4. Include guiding questions for each section

## Output Format

```markdown
# [Game Title] - Game Design Document

## Document Info
**Version:** 1.0
**Last Updated:** [Date]
**Scope:** [Prototype/Vertical Slice/Full Game]
**Target Platforms:** [Platforms]

---

## 1. Executive Summary

### High Concept
[One sentence that captures the game's essence]

### Elevator Pitch
[30-second description for stakeholders]

### Core Pillars
1. [Pillar 1] - [What this means for design decisions]
2. [Pillar 2] - [What this means for design decisions]
3. [Pillar 3] - [What this means for design decisions]

---

## 2. Gameplay

### Core Loop
[What does the player do in a 5-minute session?]

### Primary Mechanics
| Mechanic | Player Action | Purpose |
|----------|--------------|---------|
| [Name] | [What player does] | [Why it exists] |

### Secondary Mechanics
[Supporting mechanics that enhance core experience]

### Goals & Objectives
- **Short-term:** [What does player want in 5 minutes?]
- **Medium-term:** [What does player want in 1 hour?]
- **Long-term:** [What does player want overall?]

---

## 3. Progression

### Player Growth
[How does the player become more capable?]

### Content Structure
[How is content organized and unlocked?]

### Pacing
[How does intensity vary over the experience?]

---

## 4. Game World

### Setting
[Where and when does the game take place?]

### Narrative Framework
[What story structure supports gameplay?]

### Characters/Entities
[Who/what populates the world?]

---

## 5. Visual & Audio Direction

### Art Style
[Visual approach and why it fits]

### Audio Approach
[Sound design philosophy]

---

## 6. Technical Considerations

### Platform Requirements
[What does each platform need?]

### Scope Constraints
[What limitations must we design within?]

---

## 7. Appendices

### Reference Games
| Game | What We Take | What We Avoid |
|------|-------------|---------------|
| [Reference] | [Element] | [Element] |

### Open Questions
[Decisions that need to be made]

### Next Steps
[Immediate actions to move forward]
```

## Scope-Based Adjustments

**Prototype (1-2 pages):** Focus on Core Loop, Primary Mechanics, and one reference
**Vertical Slice (5-10 pages):** Add Progression, Game World basics, Visual/Audio direction
**Full GDD (20+ pages):** Complete document with detailed specifications

Adapt the depth based on user's stated scope.
