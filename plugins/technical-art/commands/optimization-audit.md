---
name: optimization-audit
description: Generate an asset optimization analysis and recommendations
---

# Optimization Audit Generator

Create an asset optimization analysis document.

## Context Gathering

Before generating the audit, understand the situation:

### Analyze Current State
- What assets exist?
- What are current metrics (triangles, textures, draw calls)?
- What's the current performance?
- What platform(s) are targeted?

### Understand Targets
- What's the frame rate target?
- What's the memory budget?
- What quality level is required?
- What are the priorities?

### Check Production Status
- How far along is the project?
- What assets are final vs. WIP?
- What's the timeline for optimization?
- Who will do the work?

### Identify Problems
- What's over budget?
- Where are the bottlenecks?
- What's causing issues?
- What's already been optimized?

Use this context to create useful audit.

## Output Format

```markdown
# Optimization Audit: [Project/Asset]

## Executive Summary
**Overall status:** [On budget / Over budget / Critical]
**Key issues:** [Top 3 problems]
**Quick wins:** [Immediate improvements]

## Current Metrics

### Performance
| Metric | Current | Budget | Status |
|--------|---------|--------|--------|
| Frame time | [Xms] | [Yms] | [Over/Under] |
| Draw calls | [X] | [Y] | [Over/Under] |
| Triangle count | [X] | [Y] | [Over/Under] |

### Memory
| Category | Current | Budget | Status |
|----------|---------|--------|--------|
| Textures | [X MB] | [Y MB] | [Over/Under] |
| Meshes | [X MB] | [Y MB] | [Over/Under] |
| Audio | [X MB] | [Y MB] | [Over/Under] |

### Load Time
| Scene | Current | Target | Status |
|-------|---------|--------|--------|
| [Scene] | [Xs] | [Ys] | [Over/Under] |

## Detailed Analysis

### Mesh Analysis
| Asset | Triangles | Draw Calls | Issue |
|-------|-----------|------------|-------|
| [Name] | [X] | [Y] | [What's wrong] |

**LOD Status:**
| Asset | Has LODs | LOD Quality |
|-------|----------|-------------|
| [Name] | [Yes/No] | [Good/Bad/None] |

### Texture Analysis
| Texture | Size | Format | Issue |
|---------|------|--------|-------|
| [Name] | [XxY] | [Format] | [What's wrong] |

**Compression Status:**
[Analysis of texture compression]

### Material Analysis
| Material | Shader | Samples | Issue |
|----------|--------|---------|-------|
| [Name] | [Shader] | [X] | [What's wrong] |

**Batching Status:**
[Analysis of draw call batching]

## Recommendations

### High Impact (Do First)
| Action | Savings | Effort | Priority |
|--------|---------|--------|----------|
| [Action] | [Metric] | [Low/Med/High] | [P0] |

### Medium Impact
| Action | Savings | Effort | Priority |
|--------|---------|--------|----------|
| [Action] | [Metric] | [Low/Med/High] | [P1] |

### Low Impact / Polish
| Action | Savings | Effort | Priority |
|--------|---------|--------|----------|
| [Action] | [Metric] | [Low/Med/High] | [P2] |

## Implementation Plan

### Phase 1: Quick Wins
**Timeline:** [Duration]
**Work:**
- [ ] [Task 1]
- [ ] [Task 2]

### Phase 2: Major Work
**Timeline:** [Duration]
**Work:**
- [ ] [Task 1]
- [ ] [Task 2]

### Phase 3: Polish
**Timeline:** [Duration]
**Work:**
- [ ] [Task 1]
- [ ] [Task 2]

## Verification

### Test Scenarios
[How to verify improvements]

### Metrics to Track
[What to measure during optimization]

## Risks
| Risk | Likelihood | Mitigation |
|------|------------|------------|
| [Risk] | [H/M/L] | [Strategy] |
```

Generate based on the user's project and optimization needs.
