---
name: test-strategy
description: Generate a test automation strategy document
---

# Test Automation Strategy Generator

Generate a comprehensive test automation strategy tailored to the game project.

## Context Gathering

Before generating, understand:

### Project Context
- Game engine and testing framework
- Game genre and complexity
- Critical systems (combat, economy, multiplayer, etc.)
- Current test coverage (if any)

### Team Context
- Team experience with testing
- Time available for test development
- CI/CD integration requirements

### Quality Goals
- Critical quality requirements
- Past bug patterns
- Release frequency

## Output Format

```markdown
# Test Automation Strategy: [Project Name]

## Overview
**Engine:** [Engine]
**Test Framework:** [Framework]
**Current Coverage:** [%] or "None"
**Target Coverage:** [%]

## Testing Philosophy

### What We Test
- Core gameplay logic (damage, movement, scoring)
- State machines and transitions
- Save/load functionality
- Economy and progression math
- Network message serialization

### What We Don't Test
- Engine functionality (Unity's Raycast, Unreal's navigation)
- Visual appearance (handled by visual regression)
- Subjective "fun" (handled by playtesting)

## Test Pyramid

```
          E2E (5%)
         /────────\
        / Integration \
       /   (15%)       \
      /─────────────────\
     /    Unit Tests     \
    /       (80%)         \
   /───────────────────────\
```

### Unit Tests (Target: [X] tests)
**Focus:** Isolated game logic
**Speed:** < 100ms each
**Examples:**
- Damage calculation
- Inventory operations
- Stat modifications

### Integration Tests (Target: [X] tests)
**Focus:** System interactions
**Speed:** < 1s each
**Examples:**
- Save/load round-trip
- Client-server message handling
- Quest state progression

### E2E Tests (Target: [X] tests)
**Focus:** Critical user flows
**Speed:** < 30s each
**Examples:**
- New player tutorial completion
- Purchase flow
- Match completion

## Test Organization

```
tests/
├── unit/
│   ├── combat/
│   ├── inventory/
│   └── progression/
├── integration/
│   ├── networking/
│   └── persistence/
├── e2e/
│   └── flows/
└── fixtures/
```

## Critical Test Areas

### Tier 1: Must Test
| System | Tests Needed | Priority |
|--------|--------------|----------|
| [Critical system] | [Types] | Immediate |

### Tier 2: Should Test
| System | Tests Needed | Priority |
|--------|--------------|----------|
| [Important system] | [Types] | This sprint |

### Tier 3: Nice to Have
| System | Tests Needed | Priority |
|--------|--------------|----------|
| [Other system] | [Types] | Backlog |

## CI Integration

### Pipeline Integration
```yaml
test-jobs:
  unit-tests:
    trigger: every push
    timeout: 5 minutes
    blocking: true

  integration-tests:
    trigger: pull requests
    timeout: 15 minutes
    blocking: true

  e2e-tests:
    trigger: nightly
    timeout: 1 hour
    blocking: false
```

### Failure Handling
- Unit test failure: Block merge
- Integration failure: Block merge
- E2E failure: Alert, investigate

## Metrics and Goals

| Metric | Current | Target | Timeline |
|--------|---------|--------|----------|
| Unit test coverage | [%] | [%] | [Date] |
| Integration coverage | [%] | [%] | [Date] |
| Flaky test rate | [%] | < 1% | [Date] |
| Test execution time | [Time] | [Time] | [Date] |

## Implementation Roadmap

### Phase 1: Foundation (Week 1-2)
1. Set up test framework
2. Create test utilities and fixtures
3. Write tests for most critical system

### Phase 2: Coverage (Week 3-6)
1. Add unit tests for core gameplay
2. Add integration tests for persistence
3. Set up CI integration

### Phase 3: Advanced (Week 7+)
1. Visual regression testing
2. Performance benchmarks
3. E2E test automation

## Resources Required

| Resource | Estimate |
|----------|----------|
| Initial setup | [Hours] |
| Test writing | [Hours/week] ongoing |
| Maintenance | [Hours/sprint] ongoing |
```

Generate the test strategy based on the project context provided.
