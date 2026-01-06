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

| Plugin | Focus | Agents | Commands |
|--------|-------|--------|----------|
| **thinking** | Creativity, mental models, biases, decision frameworks | 5 | 12 |
| **game-design** | Mechanics, systems, balance | 7 | 3 |
| **engineering** | Architecture, performance, debugging | 6 | 4 |
| **ui-ux** | Interface, onboarding, accessibility | 3 | 2 |
| **art** | Visual direction and asset planning | 2 | 2 |
| **audio** | Sound design and music | 2 | 2 |
| **product** | Product management for any product | 2 | 2 |
| **marketing** | Launch, community, and store presence | 4 | 4 |
| **operations** | Live ops, analytics, and QA | 3 | 2 |
| **strategy** | Business strategy for any venture | 3 | 2 |

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

**Commands:**
- `/code-review` — Quick code review for game development
- `/tech-spec` — Generate a technical specification
- `/pattern` — Explain a design pattern for games
- `/tech-stack` — Get advice on engine/framework selection

---

### ui-ux

User interface, user experience, and accessibility.

**Agents:**
- **interface-artisan** — Designs intuitive game interfaces
- **onboarding-guide** — Creates tutorials that teach through play
- **accessibility-advocate** — Ensures games are playable by everyone

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

Game marketing, store presence, and community building.

**Agents:**
- **launch-strategist** — Plans game launch campaigns
- **community-builder** — Builds and nurtures communities
- **aso-optimizer** — Optimizes app store presence and discoverability

**Commands:**
- `/store-page` — Review and improve store page copy
- `/announcement` — Write announcement posts
- `/trailer` — Plan a game trailer with shot list
- `/devlog` — Create development log posts

---

### operations

Live operations, analytics, and quality assurance.

**Agents:**
- **live-ops-commander** — Manages live game operations
- **analytics-interpreter** — Interprets game analytics
- **qa-planner** — Plans testing and quality assurance

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

---

## Total Toolkit

| Category | Count |
|----------|-------|
| Plugins | 10 |
| Agents | 37 |
| Commands | 35 |
| **Total Tools** | **72** |

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
