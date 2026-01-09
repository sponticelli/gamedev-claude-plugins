---
name: pcg-spec
description: Generate a procedural content generation system specification
---

# PCG Specification Generator

Create a procedural content generation system specification.

## Context Gathering

Before generating the PCG spec, understand the requirements:

### Analyze Content Needs
- What type of content is being generated?
- How much variety is needed?
- What's the quality floor?
- What's the intended playtime/replayability?

### Understand Technical Context
- When is content generated? (Load/runtime/streaming)
- What's the performance budget?
- What platforms are targeted?
- What existing systems does it integrate with?

### Check Constraints
- What must always be true about generated content?
- What should be avoided?
- What are the design pillars to maintain?
- What player expectations exist?

### Identify Scope
- What's generated vs hand-authored?
- What parameters are exposed?
- What's the seeding strategy?
- How is quality measured?

Use this context to create appropriate PCG specification.

## Output Format

```markdown
# PCG System Specification: [Content Type]

## Overview
**Content type:** [What's generated]
**Generation approach:** [Template/Grammar/Noise/etc.]
**Regeneration:** [Full/Partial/Never]
**Persistence:** [Saved/Ephemeral]

## Requirements

### Variety
**Minimum unique instances:** [Count]
**Key variation axes:** [What changes]
**Repetition tolerance:** [How soon can content repeat]

### Quality
**Quality floor:** [Minimum acceptable]
**Target quality:** [Desired level]
**Failure handling:** [Reject/Repair/Accept]

### Performance
**Generation time:** [Budget in ms]
**Memory usage:** [Budget in MB]
**Generation context:** [Load/Runtime/Background]

## Architecture

### Pipeline Overview
```
[Seed] → [Stage 1] → [Stage 2] → [Validation] → [Output]
```

### Pipeline Stages
| Stage | Input | Output | Time Budget |
|-------|-------|--------|-------------|
| [Name] | [Data type] | [Data type] | [ms] |

## Content Model

### Elements
| Element | Variations | Generation Method |
|---------|------------|-------------------|
| [Element] | [Count/Range] | [How generated] |

### Relationships
[How elements relate to each other]

### Hierarchy
[Nesting/composition structure]

## Constraints

### Hard Constraints (Must)
| Constraint | Validation | Repair |
|------------|------------|--------|
| [Rule] | [How checked] | [How fixed] |

### Soft Constraints (Should)
| Constraint | Weight | Scoring |
|------------|--------|---------|
| [Goal] | [1-10] | [How measured] |

## Seed System

### Seed Format
**Type:** [Integer/String/Compound]
**Persistence:** [Stored where/how long]
**Sharing:** [Can players share seeds?]

### Seed Derivation
[How sub-seeds are derived]

## Tuning Parameters

| Parameter | Default | Range | Effect |
|-----------|---------|-------|--------|
| [Name] | [Value] | [Min-Max] | [What changes] |

## Validation

### Critical Checks
- [ ] [Check 1]
- [ ] [Check 2]

### Quality Scoring
**Formula:** [How quality is computed]
**Threshold:** [Minimum to accept]

## Debug Features

### Visualization
[What can be visualized]

### Override Controls
[What can be manually controlled]

### Logging
[What's logged for debugging]

## Implementation Notes
[Technical considerations, dependencies, risks]
```

Generate based on the user's content and PCG requirements.
