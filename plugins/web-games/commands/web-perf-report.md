---
name: web-perf-report
description: Generate web game performance analysis report
---

# Web Performance Report Generator

Analyze and document web game performance characteristics.

## Analysis Areas

### Frame Performance
- Frame time distribution
- Frame drops and spikes
- Main thread utilization
- Render pipeline efficiency

### Memory
- JS heap usage
- Memory allocation rate
- Garbage collection frequency
- Memory leaks over time

### Loading
- Initial load time
- Asset loading waterfall
- Code splitting effectiveness
- Cache utilization

## Output Format

```markdown
# Web Performance Report: [Game Name]

## Executive Summary
**Target FPS:** 60
**Achieved FPS:** [Median]
**Frame Budget:** 16.67ms
**Median Frame Time:** [X]ms
**95th Percentile:** [X]ms

## Frame Time Analysis

### Distribution
| Range | % of Frames | Interpretation |
|-------|-------------|----------------|
| < 16ms | [%] | Smooth |
| 16-33ms | [%] | Acceptable |
| 33-50ms | [%] | Noticeable |
| > 50ms | [%] | Major hitch |

### Frame Breakdown
| Phase | Time (ms) | % of Budget |
|-------|-----------|-------------|
| Input | [X] | [%] |
| Update | [X] | [%] |
| Physics | [X] | [%] |
| Render | [X] | [%] |
| Idle | [X] | [%] |

## Memory Analysis

### Current State
| Metric | Value | Target | Status |
|--------|-------|--------|--------|
| JS Heap Used | [MB] | < [X]MB | [✓/✗] |
| JS Heap Total | [MB] | < [X]MB | [✓/✗] |
| DOM Nodes | [N] | < 1000 | [✓/✗] |
| Event Listeners | [N] | < 500 | [✓/✗] |

### Allocation Analysis
**Allocation Rate:** [KB/s]
**GC Frequency:** [N/minute]

Top Allocators:
1. [Function/Area] - [KB/frame]
2. [Function/Area] - [KB/frame]
3. [Function/Area] - [KB/frame]

## Loading Performance

### Core Web Vitals
| Metric | Value | Target | Status |
|--------|-------|--------|--------|
| FCP | [s] | < 1.5s | [✓/✗] |
| LCP | [s] | < 2.5s | [✓/✗] |
| TTI | [s] | < 3.5s | [✓/✗] |

### Asset Loading
| Asset Type | Size | Load Time | Cached |
|------------|------|-----------|--------|
| JavaScript | [MB] | [s] | [Yes/No] |
| Images | [MB] | [s] | [Yes/No] |
| Audio | [MB] | [s] | [Yes/No] |
| Other | [MB] | [s] | [Yes/No] |

## Platform Results

### Desktop
| Browser | Avg FPS | Frame Time | Memory |
|---------|---------|------------|--------|
| Chrome | [FPS] | [ms] | [MB] |
| Firefox | [FPS] | [ms] | [MB] |
| Safari | [FPS] | [ms] | [MB] |

### Mobile
| Device | Avg FPS | Frame Time | Memory |
|--------|---------|------------|--------|
| iPhone (Safari) | [FPS] | [ms] | [MB] |
| Android (Chrome) | [FPS] | [ms] | [MB] |

## Identified Bottlenecks

### Critical (Address Immediately)
1. **[Issue]** - [Impact] - [Solution]

### Important (Plan to Fix)
1. **[Issue]** - [Impact] - [Solution]

### Minor (Nice to Have)
1. **[Issue]** - [Impact] - [Solution]

## Optimization Roadmap
1. [Highest impact optimization]
2. [Second priority]
3. [Third priority]

## Monitoring Recommendations
- [Metric to track]
- [Alert threshold to set]
```

Generate performance analysis based on the profiling data provided.
