# Agent Workflow Sequences

This document describes common agent chaining patterns for different game development tasks. Each workflow shows which agents to use and in what order for maximum effectiveness.

## Feature Development Pipeline

When implementing a new game feature from concept to polish:

```
creative-catalyst    ─► Brainstorm feature ideas
       │
       ▼
mechanics-architect  ─► Design core mechanics
       │
       ▼
systems-weaver       ─► Connect to existing systems
       │
       ▼
architecture-sage    ─► Plan code architecture
       │
       ▼
gameplay-coder       ─► Implement the feature
       │
       ▼
juice-consultant     ─► Add polish and feedback
       │
       ▼
verify-implementation ─► Verify the work
```

**When to use:** Starting a new feature from scratch, major gameplay additions

---

## Polish Pipeline

When a feature works but doesn't feel right:

```
juice-consultant     ─► Diagnose feel issues
       │
       ├──────────────────┐
       ▼                  ▼
sound-architect    interface-artisan
       │                  │
       └──────────────────┤
                          ▼
              accessibility-advocate ─► Accessibility pass
                          │
                          ▼
                   verify-design ─► Verify coherence
```

**When to use:** Feature is functional but feels "flat" or lacks impact

---

## Pre-Launch Pipeline

When preparing for a game release:

```
qa-planner           ─► Create testing plan
       │
       ▼
verify-release       ─► Pre-release checklist
       │
       ├───────────────────┐
       ▼                   ▼
aso-optimizer      store-page command
       │                   │
       └───────────────────┤
                           ▼
              launch-strategist ─► Plan launch campaign
                           │
                           ▼
              community-builder ─► Prepare community
```

**When to use:** 4-8 weeks before planned release

---

## Debugging Pipeline

When tracking down and fixing bugs:

```
debug-hunter         ─► Find root cause
       │
       ├──────────────────┐
       ▼                  │ (if performance-related)
gameplay-coder            ▼
       │           performance-detective
       │                  │
       └──────────────────┤
                          ▼
                   qa-planner ─► Add regression tests
                          │
                          ▼
              verify-implementation ─► Validate fix
```

**When to use:** Mysterious bugs, hard-to-reproduce issues, performance problems

---

## Design Iteration Pipeline

When refining game design based on feedback:

```
player-psychologist  ─► Understand player motivation
       │
       ├───────────────────┬──────────────────┐
       ▼                   ▼                  ▼
balance-oracle    difficulty-tuner    economy-designer
       │                   │                  │
       └───────────────────┴──────────────────┤
                                              ▼
                                       verify-design
```

**When to use:** After playtesting, responding to player feedback

---

## Strategic Decision Pipeline

When making major project decisions:

```
bias-detector        ─► Check for cognitive biases
       │
       ▼
mental-models        ─► Apply decision frameworks
       │
       ├───────────────────┬──────────────────┐
       ▼                   ▼                  ▼
market-analyst    analytics-interpreter   scope-guardian
       │                   │                  │
       └───────────────────┴──────────────────┤
                                              ▼
                                      pivot-evaluator ─► Make the call
```

**When to use:** Pivoting, major feature cuts, business model changes

---

## Creative Ideation Pipeline

When starting something new or stuck on a problem:

```
creative-catalyst    ─► Generate initial ideas
       │
       ├───────────────────┬──────────────────┐
       ▼                   ▼                  ▼
constraint-alchemist   mash-up-maven    random-stimulus (skill)
       │                   │                  │
       └───────────────────┴──────────────────┤
                                              ▼
                                   mechanics-architect ─► Design from ideas
```

**When to use:** Game jams, breaking creative blocks, brainstorming sessions

---

## Production Planning Pipeline

When planning work and tracking progress:

```
product-owner        ─► Prioritize features
       │
       ▼
scope-guardian       ─► Validate scope
       │
       ├───────────────────┐
       ▼                   ▼
sprint-planner     asset-planner
       │                   │
       └───────────────────┤
                           ▼
                   verify-implementation ─► Track completion
```

**When to use:** Sprint planning, roadmap creation, milestone planning

---

## Art & Audio Direction Pipeline

When establishing visual and audio identity:

```
creative-catalyst    ─► Brainstorm direction options
       │
       ├───────────────────┐
       ▼                   ▼
art-director       sound-architect
       │                   │
       │                   ▼
       │            music-director
       │                   │
       └───────────────────┤
                           ▼
                   asset-planner ─► Plan production
```

**When to use:** Pre-production, establishing game identity

---

## Live Operations Pipeline

When running a live game:

```
live-ops-commander   ─► Plan events and updates
       │
       ├───────────────────┐
       ▼                   ▼
economy-designer   community-builder
       │                   │
       └───────────────────┤
                           ▼
              analytics-interpreter ─► Measure results
                           │
                           ▼
                    balance-oracle ─► Adjust based on data
```

**When to use:** Post-launch, ongoing live service games

---

## Verification Checkpoints

Verification agents should be used at key milestones:

| Milestone | Verification Agent | Purpose |
|-----------|-------------------|---------|
| Feature complete | `verify-implementation` | Code matches spec |
| Design complete | `verify-design` | Design is coherent |
| Release ready | `verify-release` | All systems go |

---

## Quick Reference: Agent Categories

| Category | Agents | Primary Focus |
|----------|--------|---------------|
| **Engineering** | architecture-sage, gameplay-coder, tools-builder, performance-detective, debug-hunter, verify-implementation | Code and systems |
| **Game Design** | mechanics-architect, systems-weaver, balance-oracle, player-psychologist, economy-designer, puzzle-architect, difficulty-tuner, verify-design | Gameplay and experience |
| **UI/UX** | interface-artisan, onboarding-guide | Player interface |
| **Accessibility** | accessibility-advocate | Inclusive design |
| **Thinking** | creative-catalyst, constraint-alchemist, mash-up-maven, bias-detector, mental-models | Problem-solving |
| **Art & Audio** | art-director, asset-planner, sound-architect, music-director | Audio/visual |
| **Product** | product-owner, sprint-planner | Planning and management |
| **Strategy** | market-analyst, business-architect, pivot-evaluator | Business decisions |
| **Marketing** | launch-strategist, community-builder, aso-optimizer | Visibility and community |
| **Operations** | live-ops-commander, analytics-interpreter, qa-planner, verify-release | Running the game |
| **Specialized** | juice-consultant, scope-guardian | Polish and focus |

---

## Tips for Effective Agent Chaining

1. **Check Related Agents sections** - Each agent has a "Related Agents" section at the end showing natural next steps
2. **Use verification agents at milestones** - Don't skip verification steps
3. **Parallel agents can run together** - Some agents complement each other when used simultaneously
4. **Context flows forward** - Later agents benefit from earlier agents' output
5. **Don't force the sequence** - Use what you need, skip what you don't
