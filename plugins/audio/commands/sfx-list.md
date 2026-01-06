---
name: sfx-list
description: Generate a structured sound effect list for a game feature or area
---

# SFX List Generator

Create a comprehensive sound effect list from a feature description.

## Output Format

```markdown
# SFX List: [Feature/Area Name]

## Summary
| Category | Count | Priority Breakdown |
|----------|-------|-------------------|
| [Category] | [#] | H:[#] M:[#] L:[#] |
**Total Unique Sounds:** [#]
**Estimated Variations:** [#]

## Player Sounds
| ID | Name | Description | Priority | Variations | Notes |
|----|------|-------------|----------|------------|-------|
| PLR_01 | [Name] | [Description] | [H/M/L] | [#] | [Notes] |

## Enemy/NPC Sounds
| ID | Name | Description | Priority | Variations | Notes |
|----|------|-------------|----------|------------|-------|
| NPC_01 | [Name] | [Description] | [H/M/L] | [#] | [Notes] |

## Environmental Sounds
| ID | Name | Description | Priority | Looping | Notes |
|----|------|-------------|----------|---------|-------|
| ENV_01 | [Name] | [Description] | [H/M/L] | [Y/N] | [Notes] |

## Object/Prop Sounds
| ID | Name | Description | Priority | Variations | Notes |
|----|------|-------------|----------|------------|-------|
| OBJ_01 | [Name] | [Description] | [H/M/L] | [#] | [Notes] |

## UI Sounds
| ID | Name | Description | Priority | Notes |
|----|------|-------------|----------|-------|
| UI_01 | [Name] | [Description] | [H/M/L] | [Notes] |

## Ambience
| ID | Name | Description | Priority | Length |
|----|------|-------------|----------|--------|
| AMB_01 | [Name] | [Description] | [H/M/L] | [mm:ss] |

## Music Cues
| ID | Name | Trigger | Type | Priority |
|----|------|---------|------|----------|
| MUS_01 | [Name] | [When plays] | [Loop/Stinger] | [H/M/L] |

## Reuse Opportunities
[Sounds that can be shared or pitch-shifted]

## Dependencies
[Sounds needed for other systems]

## Notes
[Special considerations, middleware needs, etc.]
```

Generate based on user's feature description.
