---
name: shader-brief
description: Generate a shader/material direction document
---

# Shader Brief Generator

Create a shader and material design brief.

## Context Gathering

Before generating the shader brief, understand the requirements:

### Analyze Visual Goals
- What's the art style? (Realistic, stylized, etc.)
- What's the reference imagery?
- What materials are needed?
- What special effects are required?

### Understand Technical Context
- What render pipeline? (Built-in, URP, HDRP, custom)
- What platforms? (PC, console, mobile)
- What's the shader budget?
- What existing shaders exist?

### Check Production Needs
- Who will create materials?
- What's the iteration workflow?
- How many material variations?
- Timeline for shader development?

### Identify Constraints
- Performance budget per shader?
- Minimum feature set?
- Platform-specific requirements?
- Quality tier requirements?

Use this context to design appropriate shader approach.

## Output Format

```markdown
# Shader Brief: [Material/Effect]

## Visual Goal
**Reference:** [Description or image links]
**Style:** [Realistic / Stylized / Toon / etc.]
**Key qualities:** [What makes it look right]

## Technical Context
**Pipeline:** [URP / HDRP / Built-in / Custom]
**Platforms:** [Target platforms]
**Budget:** [Performance constraints]

## Material Design

### Properties
| Property | Type | Range | Artist Control |
|----------|------|-------|----------------|
| [Name] | [Color/Float/Texture] | [Min-Max] | [Slider/Color picker/etc.] |

### Textures
| Slot | Purpose | Resolution | Format |
|------|---------|------------|--------|
| [Name] | [What it's for] | [Size] | [Compression] |

### Visual Features
| Feature | Required | Notes |
|---------|----------|-------|
| Normal mapping | [Yes/No] | [Details] |
| Emission | [Yes/No] | [Details] |
| Transparency | [Yes/No] | [Details] |
| [Custom feature] | [Yes/No] | [Details] |

## Shader Requirements

### Lighting
**Model:** [PBR / Unlit / Custom]
**Features:** [Shadows, GI, reflections, etc.]

### Special Effects
| Effect | Implementation | Trigger |
|--------|----------------|---------|
| [Effect] | [How it works] | [When it activates] |

### Quality Tiers
| Tier | Features | Cost |
|------|----------|------|
| High | [Full features] | [X samples, Y ops] |
| Medium | [Reduced] | [X samples, Y ops] |
| Low | [Minimum] | [X samples, Y ops] |

## Material Instances

### Variations Needed
| Variant | Property Changes | Use Case |
|---------|------------------|----------|
| [Name] | [What's different] | [Where used] |

### Shared Properties
[What stays constant across instances]

## Performance Target
**Texture samples:** [Max]
**Math complexity:** [Low/Med/High]
**Draw call impact:** [Batching compatible?]

## Implementation Notes
[Technical considerations, dependencies]

## Artist Workflow
**How to create:** [Process for making materials]
**Parameters to adjust:** [Key knobs for variation]
**Do not change:** [What should stay fixed]
```

Generate based on the user's visual and technical requirements.
