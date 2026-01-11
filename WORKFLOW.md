# Game Development Use Cases

A practical guide organized by what you're trying to accomplish. Find your situation, see example prompts, and get started immediately.

**How to Use This Document:**
- Browse by your current phase or challenge
- Copy example prompts directly into Claude
- Each scenario includes the recommended tools and expected output

**Quick Navigation:**
- [Starting a New Project](#starting-a-new-project)
- [Prototyping & Testing Ideas](#prototyping--testing-ideas)
- [Day-to-Day Development](#day-to-day-development)
- [Problem Solving](#problem-solving)
- [Quality and Polish](#quality-and-polish)
- [Launch Preparation](#launch-preparation)
- [Live Operations](#live-operations)
- [Quick Reference](#quick-reference)

---

## Starting a New Project

### "I have a game idea and need to validate it"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/one-page` | Command | Create a concise one-page pitch |
| `market-analyst` | Agent | Analyze market and competition |
| `/swot` | Command | Structured SWOT analysis |
| `creative-catalyst` | Agent | Expand and refine the concept |

**Example Prompts:**
```
/one-page
Create a one-page pitch for a roguelike deckbuilder where you play as a
sentient AI escaping a research facility. Target audience is hardcore
strategy fans on Steam.
```

```
I have an idea for a mobile puzzle game about gardening. Help me validate
if this is worth pursuing.
```

**What You'll Get:**
- One-page pitch document with hook, pillars, and unique selling points
- Market analysis with comparable titles and positioning opportunities
- SWOT analysis revealing strengths to leverage and risks to mitigate

**See Also:** [Creative Ideation Pipeline](WORKFLOWS.md#creative-ideation-pipeline)

---

### "I need to write a Game Design Document"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/gdd` | Command | Generate GDD structure |
| `mechanics-architect` | Agent | Detail core mechanics |
| `systems-weaver` | Agent | Connect mechanics into systems |

**Example Prompts:**
```
/gdd
Help me create a GDD for a turn-based tactics game with permadeath and
procedural missions.
```

```
I need to document the core mechanics for my action RPG. The fantasy is
"become an unstoppable force" and the core loop is fight → loot → upgrade.
```

**What You'll Get:**
- Structured GDD outline with all major sections
- Detailed mechanic specifications with parameters and edge cases
- System interaction diagrams showing how mechanics connect

---

### "I need to define my game's core pillars"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `scope-guardian` | Agent | Define and validate pillars |
| `player-psychologist` | Agent | Align pillars with player motivations |

**Example Prompts:**
```
Help me define 3-4 design pillars for my survival horror game. I want
players to feel vulnerable but resourceful.
```

```
I have these pillars for my game: "Strategic Depth", "Quick Sessions",
"Meaningful Choices". Are they specific enough?
```

**What You'll Get:**
- 3-4 well-defined pillars that guide all design decisions
- Criteria for evaluating features against pillars
- Warning signs for pillar drift

---

### "I'm stuck on the core loop"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/loop-check` | Command | Analyze loop health |
| `mechanics-architect` | Agent | Refine loop mechanics |
| `/brainstorm` | Command | Generate loop variations |

**Example Prompts:**
```
/loop-check
My core loop is: explore dungeon → fight enemies → collect gold → buy
upgrades → repeat. Something feels off.
```

```
Help me design a core loop for a cozy farming sim that can support both
5-minute and 2-hour sessions.
```

**What You'll Get:**
- Loop health diagnosis identifying weak points
- Specific improvements for pacing, tension, and reward timing
- Alternative loop structures to consider

---

### "I need to choose a tech stack or engine"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/tech-stack` | Command | Get technology recommendations |
| `architecture-sage` | Agent | Plan technical architecture |

**Example Prompts:**
```
/tech-stack
I'm a solo dev building a 2D metroidvania with pixel art. I know Python
but open to learning. Target is PC and Switch.
```

```
Help me choose between Unity and Godot for a multiplayer party game
with 4-8 players online.
```

**What You'll Get:**
- Technology recommendations with pros/cons for your situation
- Learning curve assessment
- Technical architecture considerations

---

### "I need to plan the visual style"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/style-brief` | Command | Create art direction document |
| `art-director` | Agent | Develop visual direction |
| `asset-planner` | Agent | Plan asset production |

**Example Prompts:**
```
/style-brief
I'm making a cyberpunk racing game. I want neon-drenched visuals with
retrofuturism influences. Target platform is mobile.
```

```
Help me define a visual style that's distinctive but achievable for a
2-person team.
```

**What You'll Get:**
- Art style brief with references and constraints
- Color palette and lighting direction
- Asset production priorities

---

### "I'm starting multiplayer development"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/network-spec` | Command | Network architecture document |
| `network-architect` | Agent | Design network topology |
| `netcode-specialist` | Agent | Plan latency handling |

**Example Prompts:**
```
/network-spec
I'm building a 2v2 competitive fighting game. Need low latency and
rollback netcode. Players are worldwide.
```

```
Should my co-op puzzle game use P2P or client-server? Max 4 players,
not competitive, casual audience.
```

**What You'll Get:**
- Network architecture decision document
- Latency compensation strategy
- Infrastructure requirements

**See Also:** [Multiplayer Development Pipeline](WORKFLOWS.md#multiplayer-development-pipeline)

---

### "I'm planning procedural content"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/pcg-spec` | Command | PCG system specification |
| `pcg-architect` | Agent | Design generation systems |
| `/algorithm-eval` | Command | Evaluate algorithm options |

**Example Prompts:**
```
/pcg-spec
I want procedural dungeons for my roguelike. Need distinct biomes,
guaranteed solvability, and interesting layouts.
```

```
/algorithm-eval
I need to generate procedural islands for an exploration game. Compare
noise-based vs. agent-based approaches.
```

**What You'll Get:**
- PCG system specification with generation rules
- Algorithm recommendations for your use case
- Constraint system for ensuring playable content

**See Also:** [Procedural Generation Pipeline](WORKFLOWS.md#procedural-generation-pipeline)

---

## Prototyping & Testing Ideas

### "I need to quickly prototype a mechanic"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `mechanics-architect` | Agent | Design the mechanic clearly |
| `gameplay-coder` | Agent | Implement with proper feel |
| `/juice-recipe` | Command | Add essential feedback |

**Example Prompts:**
```
Help me design a grappling hook mechanic for rapid prototyping. I need
the core parameters and feel requirements.
```

```
I want to prototype a "time rewind" mechanic. What's the minimum viable
version I should test first?
```

**What You'll Get:**
- Mechanic specification focused on testable hypothesis
- Implementation approach prioritizing iteration speed
- Minimum feedback requirements for valid testing

---

### "I want to test a game feel hypothesis"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `juice-consultant` | Agent | Define feel requirements |
| `/juice-recipe` | Command | Implementation-ready juice |

**Example Prompts:**
```
I think my dash feels sluggish. Help me test if the issue is input delay,
acceleration curve, or visual feedback.
```

```
/juice-recipe dash-attack
Create a juice recipe to make my dash attack feel impactful and satisfying.
```

**What You'll Get:**
- Testable feel hypotheses with specific variables
- A/B comparison parameters
- Implementation-ready juice specifications

---

### "I need to evaluate if this prototype is worth continuing"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `pivot-evaluator` | Agent | Objective kill/continue analysis |
| `/bias-check` | Command | Check for cognitive biases |
| `/scope-check` | Command | Evaluate scope alignment |

**Example Prompts:**
```
I've spent 2 weeks on this prototype. Players seem confused but I think
it just needs more polish. Help me evaluate objectively.
```

```
/bias-check
I want to add multiplayer to my single-player prototype because players
asked for it. Am I making the right call?
```

**What You'll Get:**
- Objective assessment with clear criteria
- Bias identification (sunk cost, scope creep, etc.)
- Kill/pivot/continue recommendation with reasoning

---

### "I'm transitioning from paper prototype to digital"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `systems-weaver` | Agent | Map systems architecture |
| `architecture-sage` | Agent | Plan code structure |

**Example Prompts:**
```
My card game works great on paper. Help me plan the digital version
without losing what makes it fun.
```

```
I playtested my board game mechanics with tokens. What should I preserve
vs. adapt for a digital version?
```

**What You'll Get:**
- System architecture mapping paper → digital
- Critical feel elements to preserve
- Digital-only enhancements to consider

---

### "I want to A/B test mechanic variations"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `ab-test-planner` | Agent | Design rigorous tests |
| `/ab-test-spec` | Command | A/B test specification |

**Example Prompts:**
```
/ab-test-spec
I have two versions of my jump mechanic: floaty vs. snappy. Design an
A/B test to determine which players prefer.
```

```
How do I test if my hard mode is "good hard" or "frustrating hard" with
limited playtesters?
```

**What You'll Get:**
- A/B test specification with hypothesis
- Required sample size and duration
- Success metrics and decision framework

---

### "I need early playtest feedback"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `playtest-coordinator` | Agent | Plan effective playtests |
| `/playtest-plan` | Command | Structured session plan |
| `ux-analyst` | Agent | Analyze findings |

**Example Prompts:**
```
/playtest-plan
I have a 15-minute prototype and 5 friends willing to test. Help me get
useful feedback without leading questions.
```

```
My playtesters said "it's fun" but I need more actionable feedback. How
do I get better data?
```

**What You'll Get:**
- Structured playtest session plan
- Observation and question techniques
- Framework for analyzing feedback

**See Also:** [User Research Pipeline](WORKFLOWS.md#user-research-pipeline)

---

## Day-to-Day Development

### "I need to design a new mechanic"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `mechanics-architect` | Agent | Design the mechanic |
| `systems-weaver` | Agent | Connect to existing systems |
| `/juice-recipe` | Command | Define game feel |

**Example Prompts:**
```
Help me design a "parry" mechanic for my action game. I want it to be
high risk/high reward and feel satisfying to master.
```

```
/juice-recipe shield-bash
I'm adding a shield bash move. Create a juice recipe for it.
```

**What You'll Get:**
- Complete mechanic specification with parameters
- Integration points with existing systems
- Feel and feedback requirements

**See Also:** [Feature Development Pipeline](WORKFLOWS.md#feature-development-pipeline)

---

### "I'm implementing a new feature"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/tech-spec` | Command | Technical specification |
| `architecture-sage` | Agent | Design clean architecture |
| `verify-implementation` | Agent | Validate the work |

**Example Prompts:**
```
/tech-spec
I need to implement an inventory system with 50 slots, stackable items,
and equipment comparison.
```

```
What's the cleanest architecture for a dialogue system that needs to
support branching, conditions, and localization?
```

**What You'll Get:**
- Technical specification document
- Architecture recommendations
- Implementation validation checklist

---

### "I need to create a new level"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/level-brief` | Command | Level design specification |
| `level-architect` | Agent | Plan layout and pacing |
| `/pacing-curve` | Command | Intensity progression |
| `encounter-designer` | Agent | Design encounters |

**Example Prompts:**
```
/level-brief
Design the third level of my platformer. It should introduce wall-jumping
and be about 5 minutes long.
```

```
/pacing-curve
Create a pacing curve for a 15-minute dungeon with 3 combat encounters
and a mini-boss.
```

**What You'll Get:**
- Level design specification with objectives
- Pacing and intensity curve
- Encounter placement and design

**See Also:** [Level Design Pipeline](WORKFLOWS.md#level-design-pipeline)

---

### "I'm writing dialogue and narrative"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/dialogue-tree` | Command | Branching dialogue structure |
| `dialogue-architect` | Agent | Design conversation flow |
| `lore-builder` | Agent | Create world-building |
| `quest-designer` | Agent | Structure quests |

**Example Prompts:**
```
/dialogue-tree
Create a branching conversation with a merchant who can be intimidated,
charmed, or bargained with.
```

```
Help me write the quest chain for finding a lost artifact. I want 3-4
steps with optional discoveries.
```

**What You'll Get:**
- Branching dialogue structure with conditions
- Character voice guidelines
- Quest structure with objectives and rewards

**See Also:** [Narrative Design Pipeline](WORKFLOWS.md#narrative-design-pipeline)

---

### "I need to design enemy or NPC behavior"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/behavior-tree` | Command | Behavior tree structure |
| `behavior-architect` | Agent | Design AI systems |
| `/npc-spec` | Command | NPC behavior specification |
| `npc-personality-designer` | Agent | Create personality |

**Example Prompts:**
```
/behavior-tree
Create a behavior tree for a patrol guard who investigates noises,
calls for backup, and searches systematically.
```

```
/npc-spec
Design a shopkeeper NPC who reacts to the player's reputation and
remembers past interactions.
```

**What You'll Get:**
- Behavior tree structure with states and transitions
- NPC specification with personality traits
- Implementation guidance

**See Also:** [AI Systems Pipeline](WORKFLOWS.md#ai-systems-pipeline)

---

### "I'm planning a sprint or milestone"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `sprint-planner` | Agent | Plan sprint capacity |
| `product-owner` | Agent | Prioritize backlog |
| `/prioritize` | Command | RICE prioritization |
| `scope-guardian` | Agent | Validate scope |

**Example Prompts:**
```
/prioritize
Prioritize these features for my next sprint: save system, boss fight,
new biome, controller support, leaderboards.
```

```
Help me plan a 2-week sprint for a 3-person team. We have the features
listed in my backlog.
```

**What You'll Get:**
- Prioritized feature list with rationale
- Sprint plan with capacity considerations
- Scope validation against pillars

**See Also:** [Production Planning Pipeline](WORKFLOWS.md#production-planning-pipeline)

---

### "I need to write user stories"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/user-story` | Command | Generate user stories |
| `product-owner` | Agent | Define acceptance criteria |

**Example Prompts:**
```
/user-story
Create user stories for an inventory system with sorting, filtering,
and quick-equip functionality.
```

**What You'll Get:**
- Well-structured user stories
- Clear acceptance criteria
- Edge cases and considerations

---

### "I need to set up CI/CD for my game"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/pipeline-spec` | Command | Pipeline specification |
| `pipeline-architect` | Agent | Design CI/CD workflow |
| `build-engineer` | Agent | Optimize builds |

**Example Prompts:**
```
/pipeline-spec
Design a CI/CD pipeline for a Unity project targeting PC, Mac, and Switch.
We use GitHub and have limited build minutes.
```

```
Our builds take 45 minutes. Help me identify optimization opportunities.
```

**What You'll Get:**
- CI/CD pipeline specification
- Build optimization recommendations
- Platform-specific considerations

---

### "I need to plan sound and music"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/audio-brief` | Command | Audio direction document |
| `sound-architect` | Agent | Design audio systems |
| `/sfx-list` | Command | Sound effect requirements |
| `music-director` | Agent | Plan music direction |

**Example Prompts:**
```
/audio-brief
Create an audio direction for a cozy farming game. I want it to feel
warm and relaxing without being sleepy.
```

```
/sfx-list
Generate a sound effect list for a combat system with melee, ranged,
and magic attacks.
```

**What You'll Get:**
- Audio direction document with references
- Sound effect requirements list
- Music and adaptive audio plans

---

## Problem Solving

### "I'm stuck creatively"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `creative-catalyst` | Agent | Break creative blocks |
| `/brainstorm` | Command | Generate 10+ ideas |
| `/random-stimulus` | Command | Force unexpected connections |
| `constraint-alchemist` | Agent | Turn limits into opportunities |
| `mash-up-maven` | Agent | Combine disparate concepts |

**Example Prompts:**
```
/brainstorm
I need 10 ideas for what happens when the player dies in my roguelike.
I want something more interesting than "restart".
```

```
/random-stimulus
I'm stuck on the theme for my puzzle game. Give me unexpected connections
to break out of my thinking.
```

```
I only have 6 months and one artist. Help me turn these constraints into
creative opportunities.
```

**What You'll Get:**
- 10+ fresh ideas for your specific problem
- Unexpected connections and mashups
- Constraint-driven creative directions

**See Also:** [Creative Ideation Pipeline](WORKFLOWS.md#creative-ideation-pipeline)

---

### "Something feels wrong with my game's balance"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `balance-oracle` | Agent | Analyze balance issues |
| `difficulty-tuner` | Agent | Calibrate difficulty |
| `economy-designer` | Agent | Fix economy problems |

**Example Prompts:**
```
Players say my game gets too easy in the mid-game. Help me diagnose and
fix the difficulty curve.
```

```
My weapon balance is off. The sword is always the best choice. How do I
make other weapons viable?
```

**What You'll Get:**
- Balance diagnosis with root cause analysis
- Specific tuning recommendations
- Progression curve adjustments

**See Also:** [Design Iteration Pipeline](WORKFLOWS.md#design-iteration-pipeline)

---

### "My game has performance problems"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `performance-detective` | Agent | Profile and diagnose |
| `asset-optimizer` | Agent | Optimize assets |
| `/optimization-audit` | Command | Asset optimization analysis |

**Example Prompts:**
```
My game drops to 20 FPS when more than 10 enemies are on screen. Help me
diagnose the issue.
```

```
/optimization-audit
Analyze my asset usage and identify optimization opportunities. I'm
targeting mobile devices.
```

**What You'll Get:**
- Performance diagnosis with profiling guidance
- Specific optimization recommendations
- Asset optimization report

---

### "I have a hard-to-find bug"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `debug-hunter` | Agent | Systematic bug investigation |
| `/code-review` | Command | Find issues in code |

**Example Prompts:**
```
Players report a crash that only happens "sometimes" after saving.
Help me track down this bug.
```

```
I have a race condition somewhere in my multiplayer code. Help me
create a strategy to find it.
```

**What You'll Get:**
- Systematic debugging approach
- Reproduction strategy
- Root cause investigation framework

**See Also:** [Debugging Pipeline](WORKFLOWS.md#debugging-pipeline)

---

### "The economy feels broken"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `economy-designer` | Agent | Design balanced economies |
| `balance-oracle` | Agent | Tune numbers |

**Example Prompts:**
```
Players are hitting the gold cap too fast. Help me fix my economy without
a full reset.
```

```
My F2P economy is either too stingy or too generous. Help me find the
balance that respects players.
```

**What You'll Get:**
- Economy diagnosis with specific issues
- Rebalancing recommendations
- Sink/source analysis

---

### "Players are confused by my tutorial"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `onboarding-guide` | Agent | Redesign onboarding |
| `interface-artisan` | Agent | Improve UI clarity |
| `/ux-audit` | Command | UX analysis |

**Example Prompts:**
```
Players keep missing the jump tutorial. They press random buttons until
something works. Help me fix this.
```

```
/ux-audit
Audit my tutorial flow. Players should learn: move, jump, attack, and
use items in the first 5 minutes.
```

**What You'll Get:**
- Tutorial redesign recommendations
- "Show don't tell" implementation strategies
- UX improvements for clarity

---

### "My feature scope keeps growing"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `scope-guardian` | Agent | Manage scope creep |
| `/scope-check` | Command | Quick scope evaluation |
| `/scope-report` | Command | Full scope analysis |

**Example Prompts:**
```
/scope-check
I want to add crafting to my action game. My pillars are "fast combat"
and "meaningful loot". Should I add this?
```

```
/scope-report
Generate a scope report for my project. We've added 15 features since
the original design.
```

**What You'll Get:**
- Scope alignment analysis
- Cut/keep recommendations
- Scope drift metrics

---

### "I need to make a big decision"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `mental-models` | Agent | Apply decision frameworks |
| `/bias-check` | Command | Check for biases |
| `/devils-advocate` | Command | Challenge your thinking |
| `/pre-mortem` | Command | Identify failure modes |
| `/first-principles` | Command | Break down to fundamentals |

**Example Prompts:**
```
/bias-check
I want to delay launch by 3 months for more polish. Am I being perfectionist
or is this the right call?
```

```
/pre-mortem
Imagine my Early Access launch failed completely. What went wrong?
```

```
/devils-advocate
I've decided to make my game free-to-play instead of premium. Challenge
this decision.
```

**What You'll Get:**
- Structured decision analysis
- Cognitive bias identification
- Counter-arguments and failure modes

**See Also:** [Strategic Decision Pipeline](WORKFLOWS.md#strategic-decision-pipeline)

---

### "Should I pivot or keep going?"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `pivot-evaluator` | Agent | Evaluate pivot decision |
| `market-analyst` | Agent | Analyze market opportunity |
| `/swot` | Command | SWOT analysis |

**Example Prompts:**
```
My roguelike has been in development for 2 years. Interest is lukewarm.
Should I pivot, persevere, or kill it?
```

```
I'm considering pivoting from premium to F2P mid-development. Help me
evaluate this decision.
```

**What You'll Get:**
- Objective pivot/persevere/kill analysis
- Market opportunity assessment
- Sunk cost bias check

---

### "My multiplayer has latency issues"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `netcode-specialist` | Agent | Diagnose and fix netcode |
| `/netcode-brief` | Command | Netcode specification |

**Example Prompts:**
```
Players complain about "rubber-banding" in my racing game. Help me
diagnose the sync issue.
```

```
My fighting game netcode works but doesn't feel responsive enough.
Players with 100ms ping struggle.
```

**What You'll Get:**
- Latency diagnosis
- Prediction/interpolation recommendations
- Rollback considerations

---

### "My web game has browser issues"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `browser-performance-expert` | Agent | Diagnose performance |
| `/webgl-audit` | Command | WebGL compatibility audit |
| `/browser-compat-matrix` | Command | Compatibility testing |

**Example Prompts:**
```
/webgl-audit
My WebGL game runs great in Chrome but crashes on Safari. Help me
diagnose the issue.
```

```
/browser-compat-matrix
Generate a browser compatibility test matrix for my HTML5 game targeting
mobile and desktop browsers.
```

**What You'll Get:**
- Browser compatibility analysis
- WebGL issue diagnosis
- Cross-browser testing matrix

---

## Quality and Polish

### "My game lacks 'juice' or feels flat"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `juice-consultant` | Agent | Diagnose feel issues |
| `/juice-audit` | Command | Comprehensive juice audit |
| `/juice-recipe` | Command | Implementation-ready juice |

**Example Prompts:**
```
/juice-audit
Audit my combat system. Attacks land but don't feel impactful. What
juice is missing?
```

```
/juice-recipe coin-collect
Create a juice recipe for collecting coins. I want that satisfying
"ka-ching" feeling.
```

**What You'll Get:**
- Diagnosis of missing game feel elements
- Prioritized juice recommendations
- Implementation-ready specifications

**See Also:** [Polish Pipeline](WORKFLOWS.md#polish-pipeline)

---

### "I need an accessibility review"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `accessibility-advocate` | Agent | Full accessibility review |
| `/a11y-check` | Command | Quick accessibility scan |
| `/a11y-plan` | Command | Implementation roadmap |

**Example Prompts:**
```
/a11y-check
Scan my game for accessibility issues. I want to reach the broadest
audience possible.
```

```
/a11y-plan
Create an accessibility implementation roadmap for my action game.
Prioritize by impact and effort.
```

**What You'll Get:**
- Accessibility issue identification
- Prioritized implementation roadmap
- Platform certification requirements

---

### "The UI needs improvement"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `interface-artisan` | Agent | Design intuitive UI |
| `/wireframe` | Command | Text-based wireframe |
| `/ux-audit` | Command | UX analysis |

**Example Prompts:**
```
/ux-audit
Audit my inventory UI. Players say it's confusing but I don't know
what specifically is wrong.
```

```
/wireframe
Create a wireframe for a skill tree that shows 50+ skills without
overwhelming the player.
```

**What You'll Get:**
- UX issue diagnosis
- UI improvement recommendations
- Wireframe concepts

---

### "I need a code quality review"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/code-review` | Command | Review code for issues |
| `architecture-sage` | Agent | Evaluate architecture |
| `/refactoring-plan` | Command | Plan refactoring |

**Example Prompts:**
```
/code-review
Review my player controller code. It works but feels like spaghetti.
```

```
/refactoring-plan
My game is 50% complete but the codebase is a mess. Help me plan a
refactoring that won't break everything.
```

**What You'll Get:**
- Code quality assessment
- Architecture recommendations
- Safe refactoring plan

---

### "I'm planning a playtest"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `playtest-coordinator` | Agent | Plan playtest sessions |
| `/playtest-plan` | Command | Session structure |
| `/survey-design` | Command | Feedback collection |

**Example Prompts:**
```
/playtest-plan
Plan a playtest for my puzzle game. I have 10 testers and 30 minutes
per session. I want to validate difficulty.
```

```
/survey-design
Design a post-playtest survey that gets actionable feedback without
leading questions.
```

**What You'll Get:**
- Structured playtest session plan
- Observation and question techniques
- Post-playtest survey design

**See Also:** [User Research Pipeline](WORKFLOWS.md#user-research-pipeline)

---

### "I need to analyze player feedback"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `ux-analyst` | Agent | Analyze UX findings |
| `player-researcher` | Agent | Interpret player data |
| `analytics-interpreter` | Agent | Combine with metrics |

**Example Prompts:**
```
I have 50 playtest responses. Help me extract actionable insights and
prioritize changes.
```

```
Players say "combat feels bad" but our metrics show good retention.
Help me reconcile this feedback.
```

**What You'll Get:**
- Categorized feedback analysis
- Actionable insights prioritized by impact
- Qualitative/quantitative reconciliation

---

### "My animations need work"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `animation-systems-designer` | Agent | Design animation systems |
| `/animation-spec` | Command | Animation specification |

**Example Prompts:**
```
/animation-spec
Create an animation specification for my character who can run, jump,
attack, take damage, and die.
```

```
My attack animations don't feel responsive. The animator says they look
fine. What's wrong?
```

**What You'll Get:**
- Animation system specification
- State machine design
- Feel-focused animation timing

---

### "I need a QA plan"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `qa-planner` | Agent | Plan testing strategy |
| `/test-strategy` | Command | Test automation strategy |

**Example Prompts:**
```
/test-strategy
Create a testing strategy for my roguelike. I need to catch balance
regressions and progression blockers.
```

```
I'm a solo dev with no QA budget. Help me create a sustainable testing
approach.
```

**What You'll Get:**
- Testing strategy document
- Automation recommendations
- Regression prevention approach

---

## Launch Preparation

### "I'm preparing for launch"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `launch-strategist` | Agent | Plan launch campaign |
| `verify-release` | Agent | Pre-release checklist |
| `/deploy-checklist` | Command | Deployment checklist |

**Example Prompts:**
```
I'm launching on Steam in 6 weeks. Help me create a launch plan with
all the moving pieces.
```

```
/deploy-checklist
Generate a deployment checklist for launching my mobile game on iOS
and Android simultaneously.
```

**What You'll Get:**
- Comprehensive launch plan
- Pre-release verification checklist
- Day-of deployment checklist

**See Also:** [Pre-Launch Pipeline](WORKFLOWS.md#pre-launch-pipeline)

---

### "I need to write store page copy"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/store-page` | Command | Store page optimization |
| `aso-optimizer` | Agent | App store optimization |

**Example Prompts:**
```
/store-page
Review and improve my Steam store description. Here's my current copy:
[paste copy]
```

```
Help me write a compelling App Store description for my puzzle game.
Target keywords: puzzle, brain teaser, relaxing.
```

**What You'll Get:**
- Optimized store page copy
- Keyword recommendations
- Screenshot and video guidance

---

### "I'm planning a trailer"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/trailer` | Command | Trailer shot planning |
| `launch-strategist` | Agent | Marketing integration |

**Example Prompts:**
```
/trailer
Plan a 60-second launch trailer for my roguelike deckbuilder. Focus on
the "one more run" hook.
```

```
I have 90 seconds of gameplay footage. Help me structure it into a
compelling trailer that shows the game's progression.
```

**What You'll Get:**
- Shot list with timing
- Capture checklist
- Music and pacing recommendations

---

### "I need platform certification"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `certification-planner` | Agent | Plan compliance |
| `/cert-checklist` | Command | Requirements checklist |
| `/compliance-audit` | Command | Check requirements |

**Example Prompts:**
```
/cert-checklist PlayStation
Generate a PlayStation TRC checklist for my action game. We're 3 months
from submission.
```

```
/compliance-audit Nintendo
Audit my Switch build against Nintendo lotcheck requirements. Flag
any potential issues.
```

**What You'll Get:**
- Platform-specific requirements checklist
- Compliance audit with issues
- Submission timeline

**See Also:** [Platform Certification Pipeline](WORKFLOWS.md#platform-certification-pipeline)

---

### "I'm preparing a pitch or press kit"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/pitch` | Command | Pitch document creation |
| `/announcement` | Command | Announcement writing |

**Example Prompts:**
```
/pitch
Create a pitch for publishers. My game is a cozy farming sim with
combat. Target: indie publishers who fund $100-500k.
```

```
/announcement
Write a press release for my game's launch date announcement. Tone:
excited but professional.
```

**What You'll Get:**
- Pitch document with key selling points
- Press release/announcement copy
- Publisher/press targeting guidance

---

### "I need a localization plan"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `localization-strategist` | Agent | Plan localization |
| `/localization-plan` | Command | Localization roadmap |

**Example Prompts:**
```
/localization-plan
Plan localization for my narrative-heavy RPG. 50,000 words of text.
Budget is limited.
```

```
Which languages should I prioritize for my mobile puzzle game? I can
afford 5 languages at launch.
```

**What You'll Get:**
- Localization roadmap and priorities
- Budget considerations
- Technical requirements

---

### "I need to plan infrastructure scaling"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `server-planner` | Agent | Plan infrastructure |
| `/server-scaling-plan` | Command | Scaling strategy |
| `/infra-plan` | Command | Infrastructure architecture |

**Example Prompts:**
```
/server-scaling-plan
Plan server scaling for my multiplayer game launch. Expecting 10k
concurrent at launch, possibly 50k if marketing works.
```

```
/infra-plan
Design infrastructure for a live service game with daily events and
seasonal content updates.
```

**What You'll Get:**
- Infrastructure architecture plan
- Scaling strategy with cost estimates
- Failover and redundancy planning

---

### "I'm launching a web game"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/pwa-spec` | Command | PWA specification |
| `/web-optimization-checklist` | Command | Launch optimization |
| `pwa-architect` | Agent | Design PWA features |

**Example Prompts:**
```
/pwa-spec
Create a PWA specification for my HTML5 puzzle game. I want offline
support and install prompts.
```

```
/web-optimization-checklist
Generate an optimization checklist for launching my browser game on
itch.io and Kongregate.
```

**What You'll Get:**
- PWA specification with service worker design
- Optimization checklist
- Cross-platform considerations

---

### "I need influencer and creator outreach"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/influencer-brief` | Command | Outreach brief |
| `community-builder` | Agent | Community strategy |

**Example Prompts:**
```
/influencer-brief
Create an influencer outreach brief for my roguelike. Target: mid-tier
YouTubers who cover indie games.
```

```
How should I approach streamers for my horror game? I want genuine
reactions, not paid promotions.
```

**What You'll Get:**
- Influencer outreach brief
- Targeting recommendations
- Collaboration approaches

---

## Live Operations

### "I'm planning a live event"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `live-ops-commander` | Agent | Plan live operations |
| `/event-spec` | Command | Event specification |
| `event-designer` | Agent | Design event systems |

**Example Prompts:**
```
/event-spec
Design a 2-week Halloween event for my mobile RPG. Include new content,
rewards, and monetization hooks.
```

```
My first live event flopped. Players engaged for day 1 then dropped off.
Help me design a better event structure.
```

**What You'll Get:**
- Event specification with timeline
- Content and reward design
- Engagement and retention hooks

**See Also:** [Live Operations Pipeline](WORKFLOWS.md#live-operations-pipeline)

---

### "I need to design a season or battle pass"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `season-architect` | Agent | Design seasonal content |
| `/season-plan` | Command | Season specification |

**Example Prompts:**
```
/season-plan
Design a 60-day battle pass for my shooter. Mix of free and premium
tracks. Target: 2 hours/day engagement.
```

```
How do I structure season progression so players feel rewarded but not
overwhelmed or FOMO-pressured?
```

**What You'll Get:**
- Season plan with progression curve
- Reward distribution strategy
- FOMO mitigation approaches

---

### "I need to analyze game metrics"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `analytics-interpreter` | Agent | Interpret metrics |
| `/metrics-report` | Command | Metrics report template |
| `/cohort-analysis` | Command | Cohort analysis framework |

**Example Prompts:**
```
/metrics-report
Help me create a weekly metrics dashboard. What KPIs should I track
for a mobile puzzle game?
```

```
/cohort-analysis
Set up a cohort analysis framework to understand how player behavior
changes over time.
```

**What You'll Get:**
- Metrics dashboard design
- KPI definitions and targets
- Cohort analysis framework

---

### "Retention is dropping"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `retention-specialist` | Agent | Diagnose retention issues |
| `/retention-audit` | Command | Retention analysis |

**Example Prompts:**
```
/retention-audit
D7 retention dropped from 25% to 18% after our last update. Help me
diagnose what went wrong.
```

```
New players drop off at level 5. What retention strategies should I
implement to get them past this wall?
```

**What You'll Get:**
- Retention diagnosis with root causes
- Improvement recommendations
- Win-back strategies

---

### "I want to run an A/B test"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `ab-test-planner` | Agent | Design tests |
| `/ab-test-spec` | Command | Test specification |

**Example Prompts:**
```
/ab-test-spec
Design an A/B test for our new tutorial. Hypothesis: animated hints
improve completion by 20%.
```

```
I want to test two pricing models. How do I design a fair test that
doesn't alienate players?
```

**What You'll Get:**
- A/B test specification
- Required sample size and duration
- Decision framework

---

### "I need to design monetization"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `monetization-strategist` | Agent | Design ethical monetization |
| `economy-designer` | Agent | Support with economy |

**Example Prompts:**
```
Help me design F2P monetization that respects players. My game is a
puzzle game with daily content.
```

```
How do I price my cosmetic shop? I don't want to feel exploitative but
I need to make money.
```

**What You'll Get:**
- Ethical monetization strategy
- Pricing recommendations
- Player perception considerations

**See Also:** [Monetization Design Pipeline](WORKFLOWS.md#monetization-design-pipeline)

---

### "I'm writing a devlog or update"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/devlog` | Command | Devlog post creation |
| `/announcement` | Command | Update announcement |
| `community-builder` | Agent | Community communication |

**Example Prompts:**
```
/devlog
Write a devlog about implementing procedural terrain. Make it technical
but accessible to non-programmers.
```

```
/announcement
Write an update announcement for a content patch. New features: 10 levels,
2 characters, balance changes.
```

**What You'll Get:**
- Engaging devlog/announcement copy
- Community tone guidance
- Call-to-action recommendations

---

### "I need to segment my players"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `player-segmentation-expert` | Agent | Define segments |
| `analytics-interpreter` | Agent | Analyze behavior |

**Example Prompts:**
```
Help me create player segments for my RPG. I want to treat whales,
dolphins, minnows, and non-payers differently.
```

```
How should I segment players by engagement pattern? I want to identify
at-risk churners.
```

**What You'll Get:**
- Player segment definitions
- Behavioral indicators
- Segment-specific strategies

---

### "Something broke in production"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/incident-response` | Command | Incident playbook |
| `deployment-coordinator` | Agent | Manage incident |

**Example Prompts:**
```
/incident-response
Create an incident response playbook for our live game. We need procedures
for server outages, economy exploits, and content bugs.
```

```
We just discovered an exploit that lets players duplicate items. What's
the incident response?
```

**What You'll Get:**
- Incident response playbook
- Severity classification
- Communication templates

---

### "I'm running a postmortem"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/postmortem` | Command | Postmortem structure |
| `analytics-interpreter` | Agent | Data analysis |

**Example Prompts:**
```
/postmortem
Structure a postmortem for our first season. It was moderately successful
but engagement dropped mid-season.
```

```
Our launch underperformed expectations. Help me run a blameless postmortem
to learn what went wrong.
```

**What You'll Get:**
- Structured postmortem framework
- Blameless analysis approach
- Actionable improvements

---

### "I'm designing guild or social features"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `guild-architect` | Agent | Design guild systems |
| `/guild-spec` | Command | Guild specification |
| `social-designer` | Agent | Design social features |
| `/social-features-plan` | Command | Social features plan |

**Example Prompts:**
```
/guild-spec
Design a guild system for my MMO. 50 max members, progression, and
guild-vs-guild competition.
```

```
/social-features-plan
Plan social features for my mobile game. I want viral mechanics without
being spammy.
```

**What You'll Get:**
- Guild system specification
- Social features design
- Viral loop considerations

**See Also:** [Social Systems Pipeline](WORKFLOWS.md#social-systems-pipeline)

---

### "I need to design matchmaking"

**Best Tools:**
| Tool | Type | Purpose |
|------|------|---------|
| `/matchmaking-spec` | Command | Matchmaking specification |
| `network-architect` | Agent | Infrastructure design |

**Example Prompts:**
```
/matchmaking-spec
Design a matchmaking system for my 1v1 fighting game. MMR-based with
casual and ranked modes.
```

```
How do I balance matchmaking between fair matches and short queue times
with a small player base?
```

**What You'll Get:**
- Matchmaking system specification
- MMR/rating system design
- Queue time optimization

---

## Quick Reference

### Commands by Task Type

| Task | Commands |
|------|----------|
| **Documents** | `/gdd`, `/tech-spec`, `/style-brief`, `/audio-brief`, `/narrative-brief`, `/level-brief` |
| **Audits** | `/juice-audit`, `/ux-audit`, `/a11y-check`, `/scope-check`, `/webgl-audit`, `/compliance-audit`, `/optimization-audit`, `/retention-audit`, `/build-audit` |
| **Specifications** | `/network-spec`, `/pcg-spec`, `/event-spec`, `/season-plan`, `/ab-test-spec`, `/guild-spec`, `/matchmaking-spec` |
| **Lists** | `/asset-list`, `/sfx-list`, `/cert-checklist`, `/deploy-checklist` |
| **Ideation** | `/brainstorm`, `/random-stimulus`, `/what-if`, `/analogy`, `/perspective` |
| **Decisions** | `/bias-check`, `/devils-advocate`, `/pre-mortem`, `/first-principles`, `/swot` |
| **Quick Outputs** | `/one-page`, `/wireframe`, `/juice-recipe`, `/trailer`, `/devlog`, `/user-story` |

### Agents by Expertise

| Area | Agents |
|------|--------|
| **Game Design** | `mechanics-architect`, `systems-weaver`, `balance-oracle`, `player-psychologist`, `puzzle-architect`, `economy-designer`, `difficulty-tuner` |
| **Engineering** | `architecture-sage`, `performance-detective`, `debug-hunter`, `gameplay-coder`, `tools-builder` |
| **Creative** | `creative-catalyst`, `constraint-alchemist`, `mash-up-maven` |
| **Production** | `product-owner`, `sprint-planner`, `scope-guardian` |
| **Art & Audio** | `art-director`, `asset-planner`, `sound-architect`, `music-director` |
| **UX** | `interface-artisan`, `onboarding-guide`, `juice-consultant`, `accessibility-advocate` |
| **Narrative** | `dialogue-architect`, `lore-builder`, `quest-designer`, `localization-strategist` |
| **Level Design** | `level-architect`, `spatial-designer`, `encounter-designer`, `environment-storyteller` |
| **Multiplayer** | `network-architect`, `netcode-specialist`, `server-planner`, `anti-cheat-architect`, `backend-developer` |
| **Technical Art** | `pipeline-architect`, `animation-systems-designer`, `asset-optimizer`, `shader-architect` |
| **AI** | `behavior-architect`, `difficulty-adapter`, `npc-personality-designer` |
| **PCG** | `pcg-architect`, `algorithm-advisor`, `constraint-designer` |
| **Operations** | `live-ops-commander`, `analytics-interpreter`, `monetization-strategist`, `event-designer`, `retention-specialist`, `season-architect` |
| **Research** | `playtest-coordinator`, `player-researcher`, `ux-analyst`, `player-segmentation-expert`, `ab-test-planner` |
| **Business** | `market-analyst`, `business-architect`, `pivot-evaluator`, `launch-strategist`, `community-builder`, `aso-optimizer` |
| **DevOps** | `pipeline-architect`, `build-engineer`, `test-automation-lead`, `infrastructure-planner`, `deployment-coordinator` |
| **Certification** | `certification-planner`, `platform-auditor`, `submission-coordinator` |
| **Web Games** | `webgl-specialist`, `browser-performance-expert`, `pwa-architect`, `web-audio-specialist`, `canvas-optimization-expert`, `web-input-handler` |
| **Social** | `guild-architect`, `social-designer` |
| **Thinking** | `bias-detector`, `mental-models` |
| **Verification** | `verify-implementation`, `verify-design`, `verify-release`, `verify-pipeline` |

### Tools by Development Phase

| Phase | Recommended Tools |
|-------|-------------------|
| **Ideation** | `/brainstorm`, `/one-page`, `/swot`, `creative-catalyst`, `market-analyst` |
| **Pre-Production** | `/gdd`, `/tech-stack`, `/style-brief`, `mechanics-architect`, `architecture-sage`, `art-director` |
| **Prototyping** | `gameplay-coder`, `/juice-recipe`, `pivot-evaluator`, `/playtest-plan` |
| **Production** | `/tech-spec`, `/level-brief`, `/behavior-tree`, `sprint-planner`, `/scope-check` |
| **Polish** | `/juice-audit`, `/a11y-plan`, `/ux-audit`, `juice-consultant`, `accessibility-advocate` |
| **Launch** | `/store-page`, `/trailer`, `/cert-checklist`, `launch-strategist`, `verify-release` |
| **Live Ops** | `/event-spec`, `/metrics-report`, `/retention-audit`, `live-ops-commander`, `analytics-interpreter` |

---

## Further Reading

- **[WORKFLOWS.md](WORKFLOWS.md)** - Agent chaining patterns for complex multi-agent workflows
- **[README.md](README.md)** - Complete catalog of all plugins, agents, and commands
