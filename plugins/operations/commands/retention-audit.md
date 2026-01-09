---
name: retention-audit
description: Analyze retention and generate improvement recommendations
---

# Retention Audit

Analyze player retention metrics and identify improvement opportunities.

## Audit Areas

### Retention Curves
- D1, D7, D14, D30 retention
- Cohort comparison
- Trend analysis

### Churn Analysis
- Drop-off points
- Churn predictors
- Segment differences

### Engagement Metrics
- Session frequency
- Session duration
- Feature engagement

## Output Format

```markdown
# Retention Audit: [Game Name]

## Executive Summary
**Audit Period:** [Date range]
**Overall Health:** [Good/Needs Attention/Critical]
**Primary Issue:** [Main retention challenge]
**Biggest Opportunity:** [Highest impact improvement]

## Retention Metrics

### Retention Curve
| Day | Current | Benchmark | Status |
|-----|---------|-----------|--------|
| D1 | [%] | 40-50% | [✓/✗] |
| D7 | [%] | 20-30% | [✓/✗] |
| D14 | [%] | 15-20% | [✓/✗] |
| D30 | [%] | 10-15% | [✓/✗] |
| D60 | [%] | 7-10% | [✓/✗] |
| D90 | [%] | 5-8% | [✓/✗] |

### Trend Analysis
| Period | D1 | D7 | D30 | Direction |
|--------|-----|-----|------|-----------|
| Current | [%] | [%] | [%] | [↑/↓/→] |
| Last month | [%] | [%] | [%] | |
| Last quarter | [%] | [%] | [%] | |

### Cohort Comparison
| Cohort | D1 | D7 | D30 | Notable |
|--------|-----|-----|------|---------|
| Organic | [%] | [%] | [%] | [Note] |
| Paid UA | [%] | [%] | [%] | [Note] |
| Viral | [%] | [%] | [%] | [Note] |

## Churn Analysis

### Primary Drop-off Points
| Stage | Drop Rate | Typical | Issue |
|-------|-----------|---------|-------|
| [Stage] | [%] | [%] | [Problem] |

### Churn Predictors
| Signal | Correlation | Detection Time |
|--------|-------------|----------------|
| [Behavior] | [%] | [Days before churn] |

### Segment Differences
| Segment | D7 Retention | Notes |
|---------|--------------|-------|
| Spenders | [%] | [Observation] |
| Non-spenders | [%] | [Observation] |
| Social players | [%] | [Observation] |
| Solo players | [%] | [Observation] |

## Engagement Analysis

### Session Metrics
| Metric | Value | Benchmark |
|--------|-------|-----------|
| Sessions/DAU | [N] | [Benchmark] |
| Avg session length | [min] | [Benchmark] |
| DAU/MAU | [%] | [Benchmark] |

### Feature Engagement
| Feature | Usage Rate | Correlation to Retention |
|---------|------------|-------------------------|
| [Feature] | [%] | [High/Med/Low] |

## Root Cause Analysis

### Issue 1: [Issue Name]
**Stage:** [Where it occurs]
**Impact:** [% of users affected]
**Evidence:** [Data supporting this]
**Hypothesis:** [Why it's happening]

### Issue 2: [Issue Name]
[Same structure]

## Recommendations

### Immediate (This Sprint)
| Action | Expected Impact | Effort |
|--------|-----------------|--------|
| [Action] | +[%] D7 | [Low/Med/High] |

### Short-Term (This Month)
| Action | Expected Impact | Effort |
|--------|-----------------|--------|
| [Action] | +[%] D30 | [Low/Med/High] |

### Long-Term (This Quarter)
| Action | Expected Impact | Effort |
|--------|-----------------|--------|
| [Action] | +[%] LTV | [Low/Med/High] |

## Monitoring Plan
| Metric | Current | Target | Check Frequency |
|--------|---------|--------|-----------------|
| [Metric] | [Value] | [Target] | [Daily/Weekly] |

## Next Steps
1. [Priority 1 action]
2. [Priority 2 action]
3. [Priority 3 action]
```

Analyze retention data and provide actionable recommendations.
