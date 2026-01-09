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

## Multiplayer Development Pipeline

When building multiplayer features:

```
network-architect    ─► Design network architecture
       │
       ▼
netcode-specialist   ─► Plan latency handling, sync
       │
       ├───────────────────┐
       ▼                   ▼
backend-developer   server-planner
       │                   │
       └───────────────────┤
                           ▼
              anti-cheat-architect ─► Security layer
                           │
                           ▼
                   verify-implementation
```

**When to use:** Adding multiplayer to any game, building online features

---

## Narrative Design Pipeline

When creating story and dialogue:

```
lore-builder         ─► Establish world foundations
       │
       ▼
quest-designer       ─► Structure player objectives
       │
       ▼
dialogue-architect   ─► Write branching conversations
       │
       ▼
localization-strategist ─► Plan for languages
       │
       ▼
environment-storyteller ─► Integrate into levels
```

**When to use:** Story-driven games, adding narrative to existing mechanics

---

## Level Design Pipeline

When designing game levels:

```
level-architect      ─► Plan overall layout and pacing
       │
       ├───────────────────┐
       ▼                   ▼
spatial-designer   encounter-designer
       │                   │
       └───────────────────┤
                           ▼
              environment-storyteller ─► Add narrative context
                           │
                           ▼
                   juice-consultant ─► Polish level feel
```

**When to use:** Creating new levels, designing tutorial sequences

---

## Technical Art Pipeline

When setting up art production:

```
pipeline-architect   ─► Design DCC-to-engine workflow
       │
       ├───────────────────┐
       ▼                   ▼
animation-systems-designer   shader-architect
       │                   │
       └───────────────────┤
                           ▼
                   asset-optimizer ─► Performance pass
                           │
                           ▼
              performance-detective ─► Validate performance
```

**When to use:** Pre-production art setup, performance optimization

---

## AI Systems Pipeline

When building game AI:

```
behavior-architect   ─► Design behavior trees/FSMs
       │
       ▼
npc-personality-designer ─► Create unique NPC behaviors
       │
       ▼
difficulty-adapter   ─► Dynamic difficulty systems
       │
       ▼
balance-oracle       ─► Tune AI challenge
       │
       ▼
verify-implementation
```

**When to use:** Creating enemy AI, NPC behaviors, adaptive systems

---

## Procedural Generation Pipeline

When building PCG systems:

```
pcg-architect        ─► Design generation system
       │
       ▼
algorithm-advisor    ─► Select appropriate algorithms
       │
       ▼
constraint-designer  ─► Define generation rules
       │
       ├───────────────────┐
       ▼                   ▼
architecture-sage   balance-oracle
       │                   │
       └───────────────────┤
                           ▼
                   verify-implementation
```

**When to use:** Roguelikes, infinite runners, procedural worlds

---

## Platform Certification Pipeline

When preparing for console/mobile release:

```
certification-planner ─► Plan compliance from start
       │
       ▼
platform-auditor     ─► Check against requirements
       │
       ▼
qa-planner           ─► Create certification test plan
       │
       ▼
submission-coordinator ─► Manage submission workflow
       │
       ▼
verify-release       ─► Final release checklist
```

**When to use:** Console releases, mobile store submissions

---

## User Research Pipeline

When gathering player feedback:

```
player-researcher    ─► Design research methodology
       │
       ├───────────────────┐
       ▼                   ▼
playtest-coordinator    survey-design (command)
       │                   │
       └───────────────────┤
                           ▼
                   ux-analyst ─► Analyze findings
                           │
                           ▼
              analytics-interpreter ─► Combine with data
                           │
                           ▼
                   interface-artisan ─► Implement improvements
```

**When to use:** Before major releases, after soft launch, ongoing research

---

## Social Systems Pipeline

When building community features:

```
social-designer      ─► Plan social feature set
       │
       ▼
guild-architect      ─► Design group systems
       │
       ├───────────────────┐
       ▼                   ▼
backend-developer   economy-designer
       │                   │
       └───────────────────┤
                           ▼
              community-builder ─► Plan community growth
                           │
                           ▼
              accessibility-advocate ─► Inclusive social features
```

**When to use:** MMOs, social games, adding clan/guild features

---

## Monetization Design Pipeline

When planning game monetization:

```
business-architect   ─► Define business model
       │
       ▼
monetization-strategist ─► Design ethical monetization
       │
       ▼
economy-designer     ─► Build supporting economy
       │
       ├───────────────────┐
       ▼                   ▼
player-psychologist   analytics-interpreter
       │                   │
       └───────────────────┤
                           ▼
                   live-ops-commander ─► Plan monetization events
```

**When to use:** F2P games, premium with IAP, subscription models

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
| **Operations** | live-ops-commander, analytics-interpreter, qa-planner, verify-release, monetization-strategist | Running the game |
| **Narrative** | dialogue-architect, lore-builder, quest-designer, localization-strategist | Story and dialogue |
| **Level Design** | level-architect, spatial-designer, encounter-designer, environment-storyteller | Spatial design |
| **Multiplayer** | network-architect, netcode-specialist, server-planner, anti-cheat-architect, backend-developer | Online systems |
| **Technical Art** | pipeline-architect, animation-systems-designer, asset-optimizer, shader-architect | Art-engineering bridge |
| **AI Systems** | behavior-architect, difficulty-adapter, npc-personality-designer | Game AI |
| **Procedural** | pcg-architect, algorithm-advisor, constraint-designer | Content generation |
| **Certification** | certification-planner, platform-auditor, submission-coordinator | Platform compliance |
| **User Research** | playtest-coordinator, player-researcher, ux-analyst | Player feedback |
| **Social Systems** | guild-architect, social-designer | Community features |
| **Specialized** | juice-consultant, scope-guardian | Polish and focus |

---

## Tips for Effective Agent Chaining

1. **Check Related Agents sections** - Each agent has a "Related Agents" section at the end showing natural next steps
2. **Use verification agents at milestones** - Don't skip verification steps
3. **Parallel agents can run together** - Some agents complement each other when used simultaneously
4. **Context flows forward** - Later agents benefit from earlier agents' output
5. **Don't force the sequence** - Use what you need, skip what you don't
