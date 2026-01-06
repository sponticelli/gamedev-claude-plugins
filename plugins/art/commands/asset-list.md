---
name: asset-list
description: Generate a structured asset list for a game feature or area
---

# Asset List Generator

Create a comprehensive asset list from a feature description.

## Output Format

```markdown
# Asset List: [Feature/Area Name]

## Summary
| Category | Count | Complexity |
|----------|-------|------------|
| [Category] | [#] | [L/M/H] |
**Total Unique Assets:** [#]
**Estimated Reuse %:** [%]

## Characters
| ID | Name | Description | Priority | Variants |
|----|------|-------------|----------|----------|
| CHR_01 | [Name] | [Brief desc] | [H/M/L] | [#] |

## Environment
| ID | Name | Description | Priority | Tileable |
|----|------|-------------|----------|----------|
| ENV_01 | [Name] | [Brief desc] | [H/M/L] | [Y/N] |

## Props
| ID | Name | Description | Priority | Interactive |
|----|------|-------------|----------|-------------|
| PRP_01 | [Name] | [Brief desc] | [H/M/L] | [Y/N] |

## VFX
| ID | Name | Description | Priority | Looping |
|----|------|-------------|----------|---------|
| VFX_01 | [Name] | [Brief desc] | [H/M/L] | [Y/N] |

## UI Elements
| ID | Name | Description | Priority | States |
|----|------|-------------|----------|--------|
| UI_01 | [Name] | [Brief desc] | [H/M/L] | [#] |

## Animation
| ID | Asset | Animation | Priority | Frames/Length |
|----|-------|-----------|----------|---------------|
| ANI_01 | [Asset ID] | [Name] | [H/M/L] | [#/sec] |

## Reuse Opportunities
[Assets that can be shared, kit-bashed, or repurposed]

## Dependencies
[Assets that block other work]

## Notes
[Special considerations]
```

Generate based on user's feature description.
