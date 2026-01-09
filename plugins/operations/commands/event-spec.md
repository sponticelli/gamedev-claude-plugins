---
name: event-spec
description: Generate specification for an in-game event
---

# Event Specification Generator

Generate a comprehensive event specification document for live operations teams.

## Context Gathering

Before generating, understand:

### Event Context
- Event type (collection, challenge, competition, narrative)
- Theme and timing (holiday, anniversary, original)
- Duration and start date
- Target audience

### Game Context
- Existing event systems
- Currency and reward types
- Content production capacity
- Technical constraints

## Output Format

```markdown
# Event Specification: [Event Name]

## Overview
**Theme:** [Theme/narrative]
**Type:** [Collection/Challenge/Competition/etc.]
**Duration:** [X days]
**Dates:** [Start] to [End]

## Narrative
[2-3 paragraph event story/theme description]

## Core Mechanics

### Primary Loop
1. [Activity player does]
2. [Reward earned]
3. [Progress made]
4. [Repeat]

### Event Currency
**Name:** [Currency name]
**Earn Rate:** [Amount per activity]
**Spend On:** [What can be purchased]
**End Handling:** [What happens to leftover]

## Progression

### Milestone Rewards
| Milestone | Requirement | Reward |
|-----------|-------------|--------|
| 1 | [Req] | [Reward] |
| 2 | [Req] | [Reward] |
| ... | ... | ... |
| Final | [Req] | [Grand prize] |

### Daily/Weekly Goals
| Goal | Requirement | Reward | Resets |
|------|-------------|--------|--------|
| [Goal] | [Req] | [Reward] | [Daily/Weekly] |

## Rewards

### Event Shop
| Item | Cost | Limit | Category |
|------|------|-------|----------|
| [Item] | [Currency] | [Max] | [Cosmetic/Currency/etc.] |

### Exclusive Items
| Item | How to Obtain | Exclusivity |
|------|---------------|-------------|
| [Item] | [Method] | [Event-only/Returns later] |

## Monetization

### Premium Offerings
| Item | Price | Contents |
|------|-------|----------|
| [Bundle] | $[X] | [Contents] |

### Value Proposition
- Free player can earn: [X]% of rewards
- Paying player advantage: [What they get]

## Technical Requirements

### New Content Needed
| Asset Type | Count | Due Date |
|------------|-------|----------|
| [Type] | [N] | [Date] |

### Development Tasks
- [ ] [Task 1]
- [ ] [Task 2]

### Config Changes
- [ ] [Config 1]
- [ ] [Config 2]

## Operations Plan

### Pre-Event
| Day | Action |
|-----|--------|
| T-14 | [Action] |
| T-7 | [Action] |
| T-1 | [Action] |

### During Event
| Day | Focus |
|-----|-------|
| 1-2 | Launch monitoring |
| Mid | Community engagement |
| Final | Completion push |

### Post-Event
- [ ] Rewards distribution
- [ ] Data collection
- [ ] Postmortem

## Success Metrics
| Metric | Target |
|--------|--------|
| Participation rate | [%] |
| Completion rate | [%] |
| Revenue | $[X] |
| Player satisfaction | [Score] |

## Risks
| Risk | Likelihood | Mitigation |
|------|------------|------------|
| [Risk] | [H/M/L] | [Plan] |
```

Generate the event specification based on the context provided.
