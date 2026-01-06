---
name: tech-spec
description: Generate a technical specification document for a game feature or system
---

# Technical Specification Generator

Create a tech spec for implementing a game feature.

## Output Format

```markdown
# Technical Spec: [Feature Name]

## Overview
**Purpose:** [What this implements]
**Design Doc Reference:** [Link to GDD section if applicable]
**Estimated Complexity:** [Low/Medium/High]

## Requirements

### Functional
- [What it must do]

### Non-Functional
- Performance: [Frame budget, memory limits]
- Platform: [Target platforms]
- Dependencies: [What it relies on]

## Architecture

### Components
| Component | Responsibility | Location |
|-----------|---------------|----------|
| [Name] | [What it does] | [Where in codebase] |

### Data Structures
```[language]
// Key data structures with comments
```

### Interfaces
```[language]
// Public interfaces
```

### Flow
[How data/control flows through the system]

## Implementation Plan

### Phase 1: Foundation
[Core functionality]
- [ ] [Task]
- [ ] [Task]

### Phase 2: Features
[Additional capabilities]
- [ ] [Task]
- [ ] [Task]

### Phase 3: Polish
[Final touches]
- [ ] [Task]
- [ ] [Task]

## Edge Cases
[Scenarios that need special handling]

## Testing Strategy
- Unit tests: [What to test]
- Integration tests: [What to verify]
- Manual tests: [Playtesting scenarios]

## Risks & Mitigations
| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| [Risk] | [L/M/H] | [L/M/H] | [How to address] |

## Open Questions
[Decisions that need to be made]
```

Generate based on the user's feature description.
