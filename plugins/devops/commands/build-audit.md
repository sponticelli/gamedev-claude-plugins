---
name: build-audit
description: Audit build system for optimization opportunities
---

# Build System Audit

Analyze the current build configuration and identify optimization opportunities.

## Context Gathering

Before auditing, understand:

### Build Environment
- Engine and version
- Build system (MSBuild, Gradle, SCons, etc.)
- Current build times (full and incremental)
- Hardware specs (CPU, RAM, storage type)

### Known Issues
- Slowest build stages
- Frequent rebuild triggers
- Cache effectiveness
- Error patterns

## Audit Checklist

### Configuration
- [ ] Parallel jobs configured appropriately
- [ ] Incremental builds enabled
- [ ] Unnecessary features disabled
- [ ] Compiler optimizations appropriate for stage

### Caching
- [ ] Build cache enabled and effective
- [ ] Cache hits vs misses tracked
- [ ] Cache size appropriate
- [ ] Cache invalidation working correctly

### Dependencies
- [ ] Dependencies are properly declared
- [ ] No circular dependencies
- [ ] Version pinning consistent
- [ ] Unused dependencies removed

### Assets
- [ ] Asset import settings optimized
- [ ] Texture compression appropriate
- [ ] Audio formats optimized
- [ ] Unnecessary assets excluded

## Output Format

```markdown
# Build Audit Report: [Project Name]

## Executive Summary
**Current Full Build:** [Time]
**Current Incremental:** [Time]
**Primary Bottleneck:** [Stage/Component]
**Estimated Improvement:** [%]

## Build Profile

### Time Breakdown
| Stage | Duration | % Total | Notes |
|-------|----------|---------|-------|
| Compilation | [Time] | [%] | [Observation] |
| Asset processing | [Time] | [%] | [Observation] |
| Linking | [Time] | [%] | [Observation] |
| Packaging | [Time] | [%] | [Observation] |

### Resource Usage
| Resource | Peak | Average | Bottleneck? |
|----------|------|---------|-------------|
| CPU | [%] | [%] | [Yes/No] |
| Memory | [GB] | [GB] | [Yes/No] |
| Disk I/O | [MB/s] | [MB/s] | [Yes/No] |

## Findings

### Quick Wins (Implement Today)
| Finding | Current | Recommended | Expected Impact |
|---------|---------|-------------|-----------------|
| [Issue] | [State] | [Fix] | [Time saved] |

### Medium Effort (This Sprint)
| Finding | Current | Recommended | Expected Impact |
|---------|---------|-------------|-----------------|
| [Issue] | [State] | [Fix] | [Time saved] |

### Long-term (Requires Planning)
| Finding | Current | Recommended | Expected Impact |
|---------|---------|-------------|-----------------|
| [Issue] | [State] | [Fix] | [Time saved] |

## Cache Analysis
**Hit Rate:** [%]
**Recommendations:**
- [Cache improvement 1]
- [Cache improvement 2]

## Recommendations Summary

### Priority Order
1. [Highest impact optimization]
2. [Second priority]
3. [Third priority]

### Expected Results
| Phase | Time Reduction | Effort |
|-------|----------------|--------|
| Quick Wins | [%] | [Hours] |
| Medium Effort | [%] | [Days] |
| Long-term | [%] | [Weeks] |
```

Analyze the build configuration and provide actionable optimization recommendations.
