---
name: metrics-report
description: Generate a structured game metrics report template or analyze provided metrics
---

# Metrics Report Generator

Create or analyze a game metrics report.

## Context Gathering

Before generating or analyzing metrics, understand the context:

### Identify Game Context
- Game type (mobile, PC, console, web)
- Business model (F2P, premium, subscription)
- Current lifecycle stage (soft launch, live, mature)
- Target audience and market

### Check for Existing Data
- Look for analytics configuration files
- Check for existing reports or dashboards
- Review previous metrics reports if available
- Identify key events being tracked

### Understand Benchmarks
- Genre-appropriate benchmarks
- Historical performance baselines
- Competitive context if known
- Target KPIs if established

### Identify Reporting Needs
- Who will read this report (team, stakeholders, investors)
- What decisions need to be informed
- Required reporting cadence
- Focus areas or concerns

Use this context to:
- Compare against appropriate benchmarks
- Focus on metrics that matter for this game type
- Tailor recommendations to the business model
- Prioritize insights based on stakeholder needs

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
