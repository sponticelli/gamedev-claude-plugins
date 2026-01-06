---
name: metrics-report
description: Generate a structured game metrics report template or analyze provided metrics
---

# Metrics Report Generator

Create or analyze a game metrics report.

## Output Format

```markdown
# Metrics Report: [Game] - [Period]

## Executive Summary
| Metric | Value | vs Last Period | vs Target | Status |
|--------|-------|----------------|-----------|--------|
| DAU | [#] | [%] | [%] | [🟢🟡🔴] |
| Revenue | [$] | [%] | [%] | [🟢🟡🔴] |
| D7 Retention | [%] | [%pt] | [%pt] | [🟢🟡🔴] |
| Session Length | [min] | [%] | [%] | [🟢🟡🔴] |

**Overall Health:** [Good/Caution/Concern]

## Engagement

### Active Users
| Metric | This Period | Last Period | Change |
|--------|-------------|-------------|--------|
| DAU | [#] | [#] | [%] |
| WAU | [#] | [#] | [%] |
| MAU | [#] | [#] | [%] |
| Stickiness | [%] | [%] | [%pt] |

### Session Metrics
[Session data]

## Retention
[Retention cohort table]

## Monetization
[Revenue metrics]

## Feature Performance
[Feature usage data]

## Key Insights
1. **[Insight]** - [Implication]
2. **[Insight]** - [Implication]
3. **[Insight]** - [Implication]

## Concerns
[Areas needing attention]

## Recommendations
| Priority | Recommendation | Expected Impact |
|----------|---------------|-----------------|
| 1 | [Action] | [Impact] |
| 2 | [Action] | [Impact] |

## Next Period Focus
[What to watch and optimize]
```

Generate report structure or analyze provided data.
