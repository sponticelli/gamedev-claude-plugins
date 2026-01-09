---
name: behavior-tree
description: Generate a behavior tree structure for NPC/enemy AI
---

# Behavior Tree Generator

Create a behavior tree design for game AI.

## Context Gathering

Before generating the behavior tree, understand the context:

### Analyze the NPC
- What type of entity? (Enemy, companion, neutral NPC)
- What's their role in gameplay?
- What actions can they perform?
- What should they prioritize?

### Understand Game Context
- What game genre and style?
- What other AI exists for reference?
- What level of complexity is appropriate?
- What debugging tools are available?

### Check Technical Requirements
- What behavior tree system is used?
- What node types are available?
- Performance constraints?
- Integration with other systems?

### Identify Key Behaviors
- What must this AI do?
- What's the highest priority?
- What's the fallback behavior?
- What triggers special behaviors?

Use this context to design appropriate behavior tree.

## Output Format

```markdown
# Behavior Tree: [NPC/Enemy Type]

## Overview
**Entity type:** [Enemy/Companion/NPC]
**Complexity:** [Simple/Medium/Complex]
**Priority focus:** [Combat/Patrol/Service/etc.]

## Tree Visualization

```
[Root: Selector]
├─ [Priority 1: Sequence]
│   ├─ [Condition]
│   └─ [Action]
├─ [Priority 2: Selector]
│   ├─ [Sequence]
│   │   ├─ [Condition]
│   │   └─ [Action]
│   └─ [Fallback]
└─ [Default: Action]
```

## Node Definitions

### Composite Nodes
| Node | Type | Children | Purpose |
|------|------|----------|---------|
| [Name] | [Selector/Sequence/Parallel] | [Names] | [What it does] |

### Condition Nodes
| Node | Check | Success | Failure |
|------|-------|---------|---------|
| [Name] | [What's evaluated] | [When true] | [When false] |

### Action Nodes
| Node | Action | Duration | Exit |
|------|--------|----------|------|
| [Name] | [What it does] | [Time/Condition] | [Success/Fail/Running] |

### Decorator Nodes
| Node | Child | Modification |
|------|-------|--------------|
| [Name] | [Which node] | [How it modifies] |

## Behavior Breakdown

### [High Priority Behavior]
**Trigger:** [What activates this branch]
**Sequence:**
1. [Check condition]
2. [Perform action]
3. [Continue or exit]

### [Medium Priority Behavior]
**Trigger:** [What activates this branch]
**Sequence:**
[Steps]

### [Fallback Behavior]
**When:** [All else fails]
**Action:** [What they do]

## Blackboard Variables
| Variable | Type | Set By | Used By |
|----------|------|--------|---------|
| [Name] | [Type] | [What sets it] | [What reads it] |

## State Transitions
[How the AI moves between major behavioral states]

## Debug Information
**Key breakpoints:** [Where to check behavior]
**Log points:** [What to log]
**Visualization:** [What to show in debug view]

## Edge Cases
| Scenario | Handling |
|----------|----------|
| [Edge case] | [How the tree handles it] |
```

Generate based on the user's NPC/enemy requirements.
