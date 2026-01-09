---
name: seed-system
description: Design a seed system for reproducible procedural generation
---

# Seed System Generator

Create a seed system design for reproducible procedural generation.

## Context Gathering

Before designing the seed system, understand the requirements:

### Analyze Reproducibility Needs
- What must be reproducible?
- Do players share seeds?
- How long must seeds work? (version stability)
- What's the debugging use case?

### Understand Content Scope
- What systems use random generation?
- How do they relate?
- What order dependencies exist?
- What's generated when?

### Check Technical Context
- What random library is used?
- What's the platform (32-bit, 64-bit)?
- Are there threading concerns?
- What's the storage format?

### Identify Features
- Player-visible seeds?
- Seed input interface?
- Cross-platform compatibility?
- Seed validation?

Use this context to design appropriate seed system.

## Output Format

```markdown
# Seed System Design: [Game/System Name]

## Overview
**Seed format:** [Integer/String/Compound]
**Visibility:** [Hidden/Visible to player]
**Sharing:** [Enabled/Disabled]
**Storage:** [Where seeds are saved]

## Seed Format

### Master Seed
**Type:** [Data type]
**Range:** [Valid values]
**Encoding:** [For display/storage]

**Example:**
```
Numeric: 1234567890
Display: "ABCD-EFGH-1234"
```

### Derived Seeds
| Subsystem | Derivation | Purpose |
|-----------|------------|---------|
| [System] | [How derived from master] | [What it seeds] |

**Derivation example:**
```
terrain_seed = hash(master_seed, "terrain")
enemy_seed = hash(master_seed, "enemies")
loot_seed = hash(master_seed, "loot")
```

## Random Number Generation

### Generator Type
**Algorithm:** [PRNG algorithm]
**Library:** [Implementation used]
**Period:** [Cycle length]

### Initialization
```
[How generator is seeded]
```

### Thread Safety
[How multiple threads are handled]

## Seed Hierarchy

```
Master Seed
├── World Seed
│   ├── Region Seeds (per region)
│   │   ├── Chunk Seeds (per chunk)
│   │   └── Feature Seeds
│   └── Event Seeds
├── Entity Seed
│   ├── Enemy Seeds
│   └── NPC Seeds
├── Loot Seed
│   ├── Chest Seeds
│   └── Drop Seeds
└── [Other Seeds]
```

## Reproducibility Rules

### Order Independence
[How to ensure order doesn't affect results]

### Isolation
[How subsystems don't affect each other]

### Versioning
[How to handle game updates]

## Player Interface

### Seed Input
**Where:** [UI location]
**Format:** [What players enter]
**Validation:** [How input is validated]

### Seed Display
**When shown:** [Conditions]
**Format:** [How displayed]
**Copy feature:** [Yes/No]

### Sharing
**Format for sharing:** [What's shared]
**Import process:** [How to use shared seed]
**Compatibility:** [Cross-version?]

## Storage

### When Saved
- [Save trigger 1]
- [Save trigger 2]

### What's Saved
| Data | Format | Location |
|------|--------|----------|
| Master seed | [Format] | [Where] |
| Derived seeds | [Format] | [Where] |
| RNG state | [Format] | [Where] |

### Migration
[How old saves work with new versions]

## Debugging

### Seed Logging
**Log format:** [What's logged]
**When logged:** [Events]

### Replay
[How to replay from seed]

### Override
[How to force specific seeds]

## Implementation Checklist

### Random Usage Rules
- [ ] Never use unseeded random
- [ ] Document all random usage
- [ ] Use derived seeds for subsystems
- [ ] Reset generator state for new generation

### Testing
- [ ] Same seed = same result (test)
- [ ] Different seeds = different results (test)
- [ ] Subsystems don't interfere (test)
- [ ] Cross-platform produces same results (if required)
```

Generate based on the user's game and seed system requirements.
