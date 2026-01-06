---
name: tech-stack
description: Get advice on choosing the right tech stack for a game project - engines, frameworks, and tools
---

# Tech Stack Advisor

Get recommendations for technology choices based on your project requirements.

## Process

1. Gather project requirements
2. Evaluate relevant options
3. Provide recommendation with reasoning

## Output Format

```markdown
# Tech Stack Recommendation: [Project Type]

## Requirements Understood
- **Target platforms:** [Platforms]
- **Game type:** [Genre, 2D/3D]
- **Team:** [Size, skills]
- **Timeline:** [Duration]
- **Special needs:** [Any specific requirements]

## Recommended Stack

### Primary Engine/Framework
**Recommendation:** [Engine]
**Why:** [Reasoning]

### Alternatives Considered
| Option | Pros | Cons | Why Not Primary |
|--------|------|------|-----------------|
| [Option] | [Pros] | [Cons] | [Reason] |

## Decision Matrix

| Factor | [Option A] | [Option B] | [Option C] |
|--------|------------|------------|------------|
| Iteration speed | [★★★/★★/★] | | |
| Target platform fit | | | |
| Team skill match | | | |
| Long-term cost | | | |
| Community/resources | | | |

## Supporting Tools
- **Version control:** [Recommendation]
- **Build/CI:** [Recommendation]
- **Audio middleware:** [If applicable]
- **Analytics:** [If applicable]

## Migration Path
[What if requirements change later]

## Red Flags to Watch
[Potential issues with chosen stack]
```

## Quick Guidance

**Web-first casual game:** TypeScript + Phaser/PixiJS
**Mobile-first 2D:** Unity or Godot
**3D game any platform:** Unity or Unreal
**Rapid prototyping:** Godot (lightest) or TypeScript (web)
**Console required:** Unity or Unreal (cert support)

## Key Questions

1. What platforms must you support?
2. 2D or 3D?
3. Performance requirements?
4. Team's existing skills?
5. Budget constraints?
6. Timeline?

Apply to user's project description.
