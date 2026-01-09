---
name: network-spec
description: Generate a network architecture decision document for a multiplayer game
---

# Network Specification Generator

Create a network architecture decision document for a multiplayer game.

## Context Gathering

Before generating the network specification, understand the project:

### Analyze Game Requirements
- What type of game is this? (FPS, RTS, MMO, casual, etc.)
- How many players per session? (2, 4-8, 8-32, 32+, MMO)
- What's the latency sensitivity? (turn-based, real-time casual, competitive)
- What platforms are targeted?

### Understand Competitive/Security Needs
- Is this competitive? How important is anti-cheat?
- What's the cheating risk level?
- Are there esports or ranked mode considerations?

### Check Existing Infrastructure
- Are there existing backend services?
- Is there a cloud provider preference?
- What's the budget range for hosting?

### Identify Session Model
- Match-based or persistent world?
- Drop-in/drop-out or fixed sessions?
- Is cross-play required?

Use this context to recommend the right network architecture.

## Output Format

```markdown
# Network Architecture Specification: [Game Name]

## Summary
**Recommended Architecture:** [Client-Server / P2P / Hybrid]
**Rationale:** [One paragraph explaining the choice]

## Requirements

### Player Requirements
| Requirement | Value |
|-------------|-------|
| Players per session | [X-Y] |
| Expected CCU at launch | [X] |
| Geographic distribution | [Regions] |
| Latency target | [Xms RTT] |

### Technical Requirements
| Requirement | Value |
|-------------|-------|
| Update rate | [X Hz] |
| Bandwidth budget | [X KB/s per player] |
| Platforms | [PC, Console, Mobile] |
| Cross-play | [Yes/No] |

### Business Requirements
| Requirement | Value |
|-------------|-------|
| Cheat prevention | [Critical/High/Medium/Low] |
| Hosting budget | [Range] |
| Time to market | [Timeline] |

## Architecture Decision

### Chosen Architecture: [Type]

**Diagram:**
[ASCII diagram of the network topology]

**How it works:**
[Brief explanation of data flow]

**Why this architecture:**
1. [Reason 1]
2. [Reason 2]
3. [Reason 3]

### Alternatives Considered

| Alternative | Why Not Chosen |
|-------------|----------------|
| [Architecture] | [Reason] |

## Authority Model

| System | Authority | Rationale |
|--------|-----------|-----------|
| Movement | [Client/Server] | [Why] |
| Combat | [Server] | [Why] |
| Inventory | [Server] | [Why] |
| [Other] | [Authority] | [Why] |

## Implementation Approach

### Phase 1: Foundation
- [ ] [Task]
- [ ] [Task]

### Phase 2: Core Features
- [ ] [Task]
- [ ] [Task]

### Phase 3: Polish
- [ ] [Task]
- [ ] [Task]

## Risks

| Risk | Likelihood | Impact | Mitigation |
|------|------------|--------|------------|
| [Risk] | [H/M/L] | [H/M/L] | [Strategy] |

## Open Questions
[Decisions that need to be made]
```

Generate based on the user's game description and requirements.
