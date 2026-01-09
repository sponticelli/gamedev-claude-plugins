---
name: npc-spec
description: Generate an NPC behavior specification
---

# NPC Specification Generator

Create a comprehensive NPC behavior specification.

## Context Gathering

Before generating the NPC spec, understand the character:

### Analyze NPC Role
- What's their function in the game?
- How does the player interact with them?
- Are they combat-capable?
- Do they have dialogue?

### Understand Context
- Where do they appear?
- What's their narrative role?
- Are they recurring or one-time?
- What factions/groups are they part of?

### Check Technical Needs
- What AI system will be used?
- What animations are available?
- What's the performance budget?
- What other NPCs exist for reference?

### Identify Personality
- What's their disposition?
- What motivates them?
- What are their quirks?
- How do they react to the player?

Use this context to create complete NPC specification.

## Output Format

```markdown
# NPC Specification: [NPC Name/Type]

## Overview
**Classification:** [Enemy/Neutral/Ally/Companion]
**Role:** [Merchant/Quest-giver/Guard/etc.]
**Location(s):** [Where they appear]
**Frequency:** [Always/Conditional/Unique]

## Identity

### Basic Info
**Name:** [Name or naming pattern]
**Appearance:** [Visual description]
**Voice:** [Vocal qualities]

### Personality
| Trait | Level | Expression |
|-------|-------|------------|
| [Trait] | [1-10] | [How it shows] |

### Motivation
**Wants:** [Goals]
**Fears:** [Avoids]
**Secret:** [Hidden aspect]

## Behaviors

### Idle State
**Default activity:** [What they do normally]
**Animations:** [Idle animation set]
**Variations:** [Different idle behaviors]
**Schedule:** [Time-based changes, if any]

### Interaction
**Player approach:** [How they react]
**Dialogue trigger:** [How to talk to them]
**Services:** [What they offer]
**Relationship tracking:** [If tracked]

### Combat (if applicable)
**Aggression:** [Passive/Defensive/Aggressive]
**Combat style:** [How they fight]
**Triggers:** [What makes them hostile]
**Allies:** [Who they fight with]
**Flee threshold:** [When they run]

### Reactions
| Trigger | Reaction |
|---------|----------|
| Player approaches | [Response] |
| Attacked | [Response] |
| Ally attacked | [Response] |
| Gift received | [Response] |
| Threat nearby | [Response] |

## Dialogue

### Voice Characteristics
**Style:** [Formal/Casual/Rough/etc.]
**Vocabulary:** [Simple/Complex]
**Quirks:** [Speech patterns]

### Key Lines
**Greeting (first):** "[Line]"
**Greeting (return):** "[Line]"
**Farewell:** "[Line]"
**Busy/dismissive:** "[Line]"
**Combat taunt:** "[Line]"

### Dialogue Trees
[Reference to dialogue content or structure]

## Technical Requirements

### AI Behavior
**System:** [FSM/BT/Other]
**Complexity:** [Simple/Medium/Complex]
**Key states:** [Main behavior states]

### Animation Requirements
| Animation | Priority | Notes |
|-----------|----------|-------|
| [Animation] | [Required/Nice-to-have] | [Details] |

### Audio Requirements
| Audio | Type | Notes |
|-------|------|-------|
| [Sound] | [VO/SFX] | [Details] |

## Spawning

### Placement
**Locations:** [Where they spawn]
**Density:** [How many]
**Conditions:** [Spawn requirements]

### Schedule
[Time-based spawn rules if any]

## Relationships

### With Player
**Starting:** [Neutral/Friendly/Hostile]
**Can change:** [Yes/No]
**Factors:** [What affects it]

### With NPCs
| NPC/Group | Relationship |
|-----------|--------------|
| [NPC] | [Friend/Neutral/Enemy] |

## Implementation Notes
[Technical considerations, dependencies, risks]
```

Generate based on the user's NPC requirements.
