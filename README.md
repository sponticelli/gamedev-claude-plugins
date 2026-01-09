# GameDev Claude Plugins

A comprehensive plugin marketplace for AI-augmented game development. These plugins provide specialized agents and commands for every discipline in game creation, from ideation to launch.

## Installation

### Add the Marketplace

```bash
claude plugin marketplace add sponticelli/gamedev-claude-plugins
```

### Install Individual Plugins

```bash
# Install all plugins
claude plugin install thinking@gamedev-claude-plugins
claude plugin install game-design@gamedev-claude-plugins
claude plugin install engineering@gamedev-claude-plugins
claude plugin install ui-ux@gamedev-claude-plugins
claude plugin install art@gamedev-claude-plugins
claude plugin install audio@gamedev-claude-plugins
claude plugin install product@gamedev-claude-plugins
claude plugin install marketing@gamedev-claude-plugins
claude plugin install operations@gamedev-claude-plugins
claude plugin install strategy@gamedev-claude-plugins
claude plugin install scope-guardian@gamedev-claude-plugins
claude plugin install juice@gamedev-claude-plugins
claude plugin install accessibility@gamedev-claude-plugins
claude plugin install narrative@gamedev-claude-plugins
claude plugin install level-design@gamedev-claude-plugins
claude plugin install multiplayer@gamedev-claude-plugins
claude plugin install technical-art@gamedev-claude-plugins
claude plugin install ai-systems@gamedev-claude-plugins
claude plugin install procedural@gamedev-claude-plugins
claude plugin install certification@gamedev-claude-plugins
claude plugin install user-research@gamedev-claude-plugins
claude plugin install social-systems@gamedev-claude-plugins
```

### Installation Scopes

Plugins can be installed at three different scope levels:

| Scope | Flag | Location | Use Case |
|-------|------|----------|----------|
| **User** | `--scope user` | `~/.claude/settings.json` | Available in ALL projects |
| **Project** | `--scope project` | `.claude/settings.json` | Shared with team via git |
| **Local** | `--scope local` | `~/.claude.json` | Current project only (default) |

#### Install Globally (All Projects)

To use plugins across all your projects, add `--scope user`:

```bash
# Add marketplace globally
claude plugin marketplace add sponticelli/gamedev-claude-plugins --scope user

# Install plugins globally
claude plugin install thinking@gamedev-claude-plugins --scope user
claude plugin install game-design@gamedev-claude-plugins --scope user
claude plugin install strategy@gamedev-claude-plugins --scope user
# ... etc
```

#### Install for Team (Project Scope)

To share plugins with your team via git:

```bash
claude plugin marketplace add sponticelli/gamedev-claude-plugins --scope project
claude plugin install game-design@gamedev-claude-plugins --scope project
```

> **Note:** If a plugin exists at multiple scopes, local overrides project, which overrides user.

## Plugins Overview

### Core Development

| Plugin | Focus | Agents | Commands |
|--------|-------|--------|----------|
| **game-design** | Mechanics, systems, balance, player psychology | 7 | 6 |
| **engineering** | Architecture, performance, debugging, refactoring | 6 | 5 |
| **art** | Visual direction and asset planning | 2 | 2 |
| **audio** | Sound design and music | 2 | 2 |

### Specialized Disciplines

| Plugin | Focus | Agents | Commands |
|--------|-------|--------|----------|
| **narrative** | Dialogue, lore, quests, localization | 4 | 4 |
| **level-design** | Layout, pacing, encounters, environmental storytelling | 4 | 4 |
| **multiplayer** | Networking, backend, anti-cheat, server infrastructure | 5 | 5 |
| **technical-art** | Pipelines, animation, shaders, optimization | 4 | 4 |
| **ai-systems** | Behavior trees, NPC design, dynamic difficulty | 3 | 4 |
| **procedural** | PCG algorithms, constraints, seed systems | 3 | 4 |
| **certification** | Platform compliance, audits, submission | 3 | 3 |
| **user-research** | Playtesting, surveys, UX analysis | 3 | 3 |
| **social-systems** | Guilds, clans, social features | 2 | 2 |

### Design & UX

| Plugin | Focus | Agents | Commands |
|--------|-------|--------|----------|
| **ui-ux** | Interface and onboarding | 2 | 2 |
| **accessibility** | Inclusive design for all players | 1 | 2 |
| **juice** | Game feel and polish | 1 | 2 |
| **scope-guardian** | Scope management and feature alignment | 1 | 2 |

### Production & Strategy

| Plugin | Focus | Agents | Commands |
|--------|-------|--------|----------|
| **thinking** | Creativity, mental models, biases, decision frameworks | 5 | 11 |
| **product** | Product management for any product | 2 | 2 |
| **marketing** | Launch, community, store presence, influencers | 3 | 5 |
| **operations** | Live ops, analytics, monetization, QA | 5 | 2 |
| **strategy** | Business strategy for any venture | 3 | 3 |

---

## Plugin Details

### thinking

Thinking tools: creativity, mental models, cognitive biases, and decision frameworks for any domain. These tools work for game design, software development, business strategy, writing, or any creative challenge.

**Agents:**
- **creative-catalyst** — Breaks creative blocks through lateral thinking techniques
- **constraint-alchemist** — Transforms limitations into creative opportunities
- **mash-up-maven** — Combines disparate concepts from different domains into novel ideas
- **bias-detector** — Identifies cognitive biases and provides debiasing strategies
- **mental-models** — Applies thinking frameworks to analyze problems and decisions

**Commands:**
- `/brainstorm` — Quick 10-idea brainstorming session on any topic
- `/reverse` — Apply assumption reversal technique
- `/what-if` — Explore hypothetical scenarios
- `/random-stimulus` — Use random inputs to force unexpected connections
- `/analogy` — Import solutions from distant domains
- `/perspective` — View problems through different user personas
- `/bias-check` — Quick scan for cognitive biases affecting a decision
- `/devils-advocate` — Build the strongest case against your current thinking
- `/pre-mortem` — Imagine failure and work backwards to prevent it
- `/first-principles` — Break down to fundamental truths and rebuild
- `/second-order` — Think through consequences of consequences
- `/inversion` — Flip the problem to find what guarantees failure

---

### game-design

Core game design—mechanics, systems, balance, and player experience.

**Agents:**
- **mechanics-architect** — Designs and refines core game mechanics
- **systems-weaver** — Creates interconnected game systems
- **balance-oracle** — Analyzes and improves game balance
- **player-psychologist** — Applies player psychology to design
- **puzzle-architect** — Designs puzzles and difficulty curves
- **economy-designer** — Creates sustainable in-game economies
- **difficulty-tuner** — Calibrates challenge and accessibility

**Commands:**
- `/gdd` — Generate a Game Design Document outline
- `/one-page` — Create a one-page game pitch
- `/loop-check` — Analyze core loop health

---

### engineering

Game programming, architecture, and technical problem-solving.

**Agents:**
- **architecture-sage** — Designs clean, scalable game architecture
- **performance-detective** — Investigates and solves performance problems
- **debug-hunter** — Tracks down bugs through systematic investigation
- **gameplay-coder** — Implements mechanics with proper feel
- **tools-builder** — Creates internal tools and dev workflows
- **verify-implementation** — Verifies code matches specifications

**Commands:**
- `/code-review` — Quick code review for game development
- `/tech-spec` — Generate a technical specification
- `/pattern` — Explain a design pattern for games
- `/tech-stack` — Get advice on engine/framework selection
- `/refactoring-plan` — Create structured approach for code refactoring

---

### ui-ux

User interface, user experience, and player onboarding.

**Agents:**
- **interface-artisan** — Designs intuitive game interfaces
- **onboarding-guide** — Creates tutorials that teach through play

**Commands:**
- `/wireframe` — Generate text-based UI wireframe
- `/ux-audit` — Quick UX audit of a feature

---

### art

Visual direction, style guides, and asset production.

**Agents:**
- **art-director** — Develops visual direction and style guides
- **asset-planner** — Plans art asset production and pipelines

**Commands:**
- `/style-brief` — Quick art style brief
- `/asset-list` — Generate structured asset list

---

### audio

Sound design, music, and audio implementation.

**Agents:**
- **sound-architect** — Designs game audio systems
- **music-director** — Plans music and adaptive audio

**Commands:**
- `/audio-brief` — Quick audio direction brief
- `/sfx-list` — Generate sound effect list

---

### product

Product management, prioritization, and planning for any product. Works for software, services, or physical products.

**Agents:**
- **product-owner** — Manages vision, prioritization, and stakeholder communication
- **sprint-planner** — Plans sprints, capacity, and agile ceremonies

**Commands:**
- `/user-story` — Generate well-structured user story with acceptance criteria
- `/prioritize` — Prioritize features using RICE framework

---

### marketing

Game marketing, store presence, community building, and influencer outreach.

**Agents:**
- **launch-strategist** — Plans game launch campaigns
- **community-builder** — Builds and nurtures communities
- **aso-optimizer** — Optimizes app store presence and discoverability

**Commands:**
- `/store-page` — Review and improve store page copy
- `/announcement` — Write announcement posts
- `/trailer` — Plan a game trailer with shot list
- `/devlog` — Create development log posts
- `/influencer-brief` — Create influencer outreach and collaboration brief

---

### operations

Live operations, analytics, monetization, and quality assurance.

**Agents:**
- **live-ops-commander** — Manages live game operations
- **analytics-interpreter** — Interprets game analytics
- **qa-planner** — Plans testing and quality assurance
- **verify-release** — Pre-release verification checklist
- **monetization-strategist** — Designs ethical monetization strategies

**Commands:**
- `/postmortem` — Structure a project postmortem
- `/metrics-report` — Generate metrics report template

---

### strategy

Business strategy, market analysis, and decision-making for any venture. Startups, projects, career decisions, or established businesses.

**Agents:**
- **market-analyst** — Analyzes markets, competition, and positioning opportunities
- **business-architect** — Designs business models and revenue strategies
- **pivot-evaluator** — Evaluates whether to pivot, persevere, or kill a project

**Commands:**
- `/pitch` — Create a pitch document for investors or stakeholders
- `/swot` — Generate SWOT analysis with strategic implications

---

### scope-guardian

Scope management—tracks features against design pillars, detects scope creep, and protects project focus. Essential for keeping projects on track and finishing what you started.

**Agents:**
- **scope-guardian** — Evaluates features against design pillars, calculates scope drift, identifies creep patterns

**Commands:**
- `/scope-check` — Quick check if a feature aligns with pillars
- `/scope-report` — Full scope drift analysis with metrics and recommendations

---

### juice

Game feel and polish—screen shake, particles, animation easing, audio feedback, and the secret sauce that makes games satisfying. Based on principles from "The Art of Screen Shake" and game feel best practices.

**Agents:**
- **juice-consultant** — Diagnoses missing game feel and prescribes specific juice treatments

**Commands:**
- `/juice-audit` — Analyze a feature for missing juice
- `/juice-recipe` — Get implementation-ready juice recipe for a mechanic

---

### accessibility

Game accessibility—ensuring games are playable by everyone through visual, motor, cognitive, and auditory accommodations. Combines WCAG, Game Accessibility Guidelines, and platform certification requirements.

**Agents:**
- **accessibility-advocate** — Reviews accessibility across all pillars, identifies barriers, prioritizes fixes

**Commands:**
- `/a11y-check` — Quick accessibility scan of a feature
- `/a11y-plan` — Full accessibility implementation roadmap

---

### narrative

Narrative design—dialogue, world-building, quests, and localization.

**Agents:**
- **dialogue-architect** — Designs branching dialogue and conversation systems
- **lore-builder** — Creates world-building and environmental storytelling
- **quest-designer** — Structures quests, objectives, and rewards
- **localization-strategist** — Plans localization and cultural adaptation

**Commands:**
- `/dialogue-tree` — Generate branching dialogue structure
- `/narrative-brief` — Quick narrative direction document
- `/localization-plan` — Localization strategy and execution plan
- `/world-bible` — Generate world-building foundation document

---

### level-design

Level design—spatial design, pacing, and environmental storytelling.

**Agents:**
- **level-architect** — Plans level layout, pacing, and progression
- **spatial-designer** — Designs spaces, sightlines, and navigation flow
- **encounter-designer** — Designs combat/puzzle encounters within levels
- **environment-storyteller** — Integrates narrative through environment

**Commands:**
- `/level-brief` — Quick level design specification
- `/layout-wireframe` — Text-based level layout description
- `/pacing-curve` — Level pacing and intensity curve
- `/encounter-spec` — Single encounter design specification

---

### multiplayer

Multiplayer systems—networking, backend development, and online infrastructure.

**Agents:**
- **network-architect** — Designs client-server, P2P, or hybrid architecture
- **netcode-specialist** — Handles latency, prediction, interpolation, sync
- **server-planner** — Plans infrastructure, scaling, regional deployment
- **anti-cheat-architect** — Designs validation and security measures
- **backend-developer** — Implements server-side game logic and services

**Commands:**
- `/network-spec` — Network architecture decision document
- `/netcode-brief` — Low-level networking specification
- `/server-scaling-plan` — Infrastructure and scaling strategy
- `/matchmaking-spec` — Matchmaking system design
- `/rpc-design` — RPC/messaging system design

---

### technical-art

Technical art—bridging art and engineering through pipelines, shaders, and optimization.

**Agents:**
- **pipeline-architect** — Plans DCC-to-engine workflows and automation
- **animation-systems-designer** — Designs rigs, state machines, blend trees
- **asset-optimizer** — Optimizes models, textures, LODs for performance
- **shader-architect** — Plans materials, shaders, rendering techniques

**Commands:**
- `/art-pipeline-spec` — Art production pipeline specification
- `/animation-spec` — Animation system and state machine design
- `/optimization-audit` — Asset optimization analysis
- `/shader-brief` — Shader/material direction document

---

### ai-systems

Game AI—behavior trees, NPC design, and adaptive systems.

**Agents:**
- **behavior-architect** — Designs NPC behavior trees and state machines
- **difficulty-adapter** — Designs dynamic difficulty adjustment systems
- **npc-personality-designer** — Creates NPC personality and reactions

**Commands:**
- `/behavior-tree` — Generate behavior tree structure
- `/npc-spec` — NPC behavior specification
- `/difficulty-curve` — Dynamic difficulty system design
- `/ai-architecture` — AI system architecture overview

---

### procedural

Procedural content generation—algorithms, constraints, and seed systems.

**Agents:**
- **pcg-architect** — Designs procedural content generation systems
- **algorithm-advisor** — Matches PCG algorithms to use cases
- **constraint-designer** — Designs rule systems for procedural content

**Commands:**
- `/pcg-spec` — Procedural generation system specification
- `/algorithm-eval` — Evaluate which PCG algorithm fits needs
- `/constraint-rules` — Content generation constraints and rules
- `/seed-system` — Design reproducible seed system

---

### certification

Platform certification—TRC/XR compliance, audits, and submission.

**Agents:**
- **certification-planner** — Plans compliance from project start
- **platform-auditor** — Audits against platform-specific requirements
- **submission-coordinator** — Manages submission workflow and timing

**Commands:**
- `/cert-checklist` — Platform-specific certification requirements
- `/compliance-audit` — Check against platform requirements
- `/submission-plan` — Timeline for platform submissions

---

### user-research

User research—playtesting, surveys, and UX analysis.

**Agents:**
- **playtest-coordinator** — Plans and runs playtesting sessions
- **player-researcher** — Designs surveys, interviews, and analysis
- **ux-analyst** — Analyzes player behavior and identifies pain points

**Commands:**
- `/playtest-plan` — Structured playtesting session plan
- `/survey-design` — Player survey with effective question design
- `/research-brief` — Quick player research objective document

---

### social-systems

Social systems—guilds, clans, and in-game social features.

**Agents:**
- **guild-architect** — Designs clan/guild systems and group mechanics
- **social-designer** — Plans social features, communication, and sharing

**Commands:**
- `/guild-spec` — Guild/clan system specification
- `/social-features-plan` — In-game social features design

---

## Design Philosophy

### Tech-Stack Agnostic
All agents and commands work regardless of engine (Unity, Unreal, Godot, custom) or programming language. Focus is on principles and processes that apply universally.

### Scale Agnostic
Whether you're a solo indie developer or part of a large studio, these tools adapt to your context. Agents provide frameworks that scale up or down.

### Practical Over Theoretical
Every agent includes concrete processes, templates, and actionable outputs. Theory is included only when it informs practice.

---

## Example Usage

### Creative Ideation
```
You: /random-stimulus

Claude: [Generates random stimuli and forces unexpected connections to your game problem]
```

### Game Design
```
You: Help me design the economy for my mobile puzzle game

Claude: [Uses economy-designer agent to create sustainable currency and progression]
```

### Technical Architecture
```
You: /tech-stack

Claude: [Analyzes your requirements and recommends engine/framework choices]
```

### Marketing
```
You: /trailer

Claude: [Creates a structured trailer plan with shot list and capture checklist]
```

### Strategic Decision
```
You: I'm not sure if I should continue with this project

Claude: [Uses pivot-evaluator agent to help you make a clear-eyed assessment]
```

### Multiplayer Architecture
```
You: /network-spec

Claude: [Analyzes requirements and designs client-server vs P2P architecture]
```

### Narrative Design
```
You: Help me create a branching dialogue system for my RPG

Claude: [Uses dialogue-architect agent to design conversation trees and voice]
```

### Level Design
```
You: /pacing-curve

Claude: [Creates intensity and pacing curve for level progression]
```

### Platform Certification
```
You: /cert-checklist PlayStation

Claude: [Generates PlayStation TRC requirements checklist]
```

---

## Total Toolkit

| Category | Count |
|----------|-------|
| Plugins | 22 |
| Agents | 71 |
| Commands | 73 |
| **Total Tools** | **144** |

---

## Contributing

Contributions welcome! Please submit PRs for:
- New agents or commands
- Improvements to existing content
- Bug fixes in templates or frameworks
- Documentation improvements

---

## License

MIT License - See [LICENSE](LICENSE) for details.
