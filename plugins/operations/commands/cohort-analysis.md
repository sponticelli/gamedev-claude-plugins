---
name: cohort-analysis
description: Generate cohort analysis framework
---

# Cohort Analysis Framework

Generate a framework for analyzing player cohorts over time.

## Context Gathering

Before generating, understand:

### Analysis Goals
- What questions to answer
- Key decisions to inform
- Time period of interest

### Available Data
- Cohort definitions possible
- Metrics available
- Historical depth

## Output Format

```markdown
# Cohort Analysis: [Game Name]

## Analysis Overview
**Period:** [Date range]
**Cohort Type:** [Install date/First purchase/Feature unlock/etc.]
**Primary Question:** [What we're trying to understand]

## Cohort Definitions

### Primary Cohorts
| Cohort | Definition | Size | Purpose |
|--------|------------|------|---------|
| [Name] | [Criteria] | [N users] | [Why analyze] |

### Time Periods
| Period | Dates | Notes |
|--------|-------|-------|
| Week 1 | [Dates] | [Context] |
| Week 2 | [Dates] | [Context] |
| ... | ... | ... |

## Retention Analysis

### Retention Grid
| Cohort | D1 | D7 | D14 | D30 | D60 |
|--------|-----|-----|------|------|------|
| Week 1 | [%] | [%] | [%] | [%] | [%] |
| Week 2 | [%] | [%] | [%] | [%] | [-] |
| Week 3 | [%] | [%] | [%] | [-] | [-] |
| Week 4 | [%] | [%] | [-] | [-] | [-] |

### Retention Trends
| Metric | Trend | Significance |
|--------|-------|--------------|
| D1 | [↑/↓/→] | [Notable change?] |
| D7 | [↑/↓/→] | [Notable change?] |
| D30 | [↑/↓/→] | [Notable change?] |

## Monetization Analysis

### Revenue by Cohort
| Cohort | D7 ARPU | D30 ARPU | D60 ARPU | Projected LTV |
|--------|---------|----------|----------|---------------|
| [Cohort] | $[X] | $[X] | $[X] | $[X] |

### Conversion by Cohort
| Cohort | D7 Conv | D30 Conv | Avg First Purchase |
|--------|---------|----------|-------------------|
| [Cohort] | [%] | [%] | $[X] |

### Spend Distribution
| Cohort | % Non-Spender | % Minnow | % Dolphin | % Whale |
|--------|---------------|----------|-----------|---------|
| [Cohort] | [%] | [%] | [%] | [%] |

## Engagement Analysis

### Sessions by Cohort
| Cohort | D1 Sessions | D7 Sessions | D30 Sessions |
|--------|-------------|-------------|--------------|
| [Cohort] | [N] | [N] | [N] |

### Time Spent
| Cohort | D1 Minutes | D7 Daily Avg | D30 Daily Avg |
|--------|------------|--------------|---------------|
| [Cohort] | [N] | [N] | [N] |

## Behavioral Analysis

### Feature Adoption
| Feature | Cohort 1 | Cohort 2 | Cohort 3 | Correlation |
|---------|----------|----------|----------|-------------|
| [Feature] | [%] | [%] | [%] | [to retention] |

### Progression
| Milestone | Cohort 1 | Cohort 2 | Cohort 3 |
|-----------|----------|----------|----------|
| Tutorial complete | [%] | [%] | [%] |
| Level 10 | [%] | [%] | [%] |
| First purchase | [%] | [%] | [%] |

## Comparison Analysis

### What Changed Between Cohorts
| Factor | Cohort 1 | Cohort 2 | Impact |
|--------|----------|----------|--------|
| [Game version] | [v1.0] | [v1.1] | [Metrics affected] |
| [UA source] | [Mix] | [Mix] | [Quality change] |
| [Season] | [Summer] | [Fall] | [Engagement shift] |

### Attribution
| Change | Likely Cause | Confidence |
|--------|--------------|------------|
| D7 +5% | [Feature X released] | [High/Med/Low] |
| LTV -10% | [UA quality drop] | [High/Med/Low] |

## Key Insights

### Finding 1: [Title]
**Observation:** [What the data shows]
**Hypothesis:** [Why this might be happening]
**Recommendation:** [What to do about it]

### Finding 2: [Title]
[Same structure]

### Finding 3: [Title]
[Same structure]

## Recommendations

### Immediate Actions
1. [Action based on cohort analysis]
2. [Action based on cohort analysis]

### Further Analysis Needed
1. [Deeper dive required]
2. [Additional data needed]

### Success Metrics
| Metric | Current (Latest Cohort) | Target | Timeline |
|--------|------------------------|--------|----------|
| [Metric] | [Value] | [Target] | [When] |

## Methodology Notes

### Data Quality
- [Any caveats about the data]
- [Known limitations]

### Statistical Notes
- Sample sizes by cohort
- Confidence intervals
- Significance thresholds used
```

Analyze cohort data and provide actionable insights.
