---
name: ai-architecture
description: Generate an AI system architecture overview
---

# AI Architecture Generator

Create an AI system architecture overview document.

## Context Gathering

Before generating the AI architecture, understand the project:

### Analyze AI Needs
- What types of AI entities exist?
- How many simultaneous AI actors?
- What's the complexity range?
- What shared behaviors exist?

### Understand Technical Context
- What engine/framework?
- What existing AI systems to work with?
- Performance budget for AI?
- Debugging requirements?

### Check Patterns
- What AI architecture pattern? (FSM, BT, Utility, GOAP)
- What's the perception system?
- What's the navigation system?
- How do AI communicate?

### Identify Requirements
- Must-have AI features?
- Nice-to-have AI features?
- Reusability requirements?
- Extension points needed?

Use this context to design appropriate AI architecture.

## Output Format

```markdown
# AI Architecture: [Game Name]

## Overview
**Primary pattern:** [FSM/BT/Utility/GOAP/Hybrid]
**Entity types:** [Number and types of AI]
**Max simultaneous:** [Concurrent AI count]
**Performance budget:** [CPU/memory allocation]

## System Diagram

```
┌─────────────────────────────────────────┐
│              AI Director                │
│  (Spawning, Distribution, Difficulty)   │
└─────────────────┬───────────────────────┘
                  │
    ┌─────────────┼─────────────┐
    ▼             ▼             ▼
┌────────┐  ┌────────┐  ┌────────┐
│ Agent  │  │ Agent  │  │ Agent  │
│ Brain  │  │ Brain  │  │ Brain  │
└───┬────┘  └───┬────┘  └───┬────┘
    │           │           │
    ▼           ▼           ▼
┌─────────────────────────────────────────┐
│           Shared Systems                │
│  (Perception, Navigation, Blackboard)  │
└─────────────────────────────────────────┘
```

## Core Components

### AI Director
**Purpose:** [Global AI management]
**Responsibilities:**
- [Responsibility 1]
- [Responsibility 2]

### Agent Brain
**Purpose:** [Individual decision making]
**Architecture:** [FSM/BT/etc.]
**Update rate:** [Hz or event-driven]

### Perception System
**Senses:** [Sight, hearing, etc.]
**Update rate:** [Hz]
**Culling:** [How perception is optimized]

### Navigation System
**Pathfinding:** [NavMesh/Grid/etc.]
**Steering:** [How movement is controlled]
**Avoidance:** [How agents avoid each other]

### Blackboard System
**Scope:** [Per-agent/Shared/Both]
**Data types:** [What's stored]
**Persistence:** [How long data lives]

## Entity Types

| Type | Brain Type | Complexity | Count |
|------|------------|------------|-------|
| [Type] | [FSM/BT/etc.] | [Simple/Med/Complex] | [Typical count] |

## Behavior Sharing

### Shared Components
| Component | Used By | Purpose |
|-----------|---------|---------|
| [Component] | [Entity types] | [What it does] |

### Behavior Library
[Reusable behavior patterns]

## Communication

### Agent-to-Agent
**Method:** [Direct/Event/Blackboard]
**Types:** [What's communicated]

### Agent-to-System
**Events up:** [What agents report]
**Commands down:** [What systems command]

## Performance

### Budgets
| System | Budget | Notes |
|--------|--------|-------|
| Perception | [Xms] | [Per-frame/Distributed] |
| Decision | [Xms] | [Per-frame/Distributed] |
| Navigation | [Xms] | [Per-frame/Distributed] |

### Optimization Strategies
- [LOD for distant AI]
- [Staggered updates]
- [Perception culling]
- [Cached decisions]

## Debugging

### Visualization
[What's shown in debug mode]

### Logging
[What's logged, log levels]

### Tools
[Debug tools available]

## Extension Points

### Adding New Entities
[How to add new AI types]

### Adding New Behaviors
[How to add new behaviors]

### Customization
[What can be tuned/configured]

## Implementation Phases

### Phase 1: Foundation
- [ ] [Core system 1]
- [ ] [Core system 2]

### Phase 2: Entity Types
- [ ] [Entity type 1]
- [ ] [Entity type 2]

### Phase 3: Polish
- [ ] [Polish item 1]
- [ ] [Polish item 2]
```

Generate based on the user's game and AI requirements.
