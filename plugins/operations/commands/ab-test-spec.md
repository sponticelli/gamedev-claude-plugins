---
name: ab-test-spec
description: Generate A/B test specification
---

# A/B Test Specification Generator

Generate a rigorous A/B test specification document.

## Context Gathering

Before generating, understand:

### Test Context
- What feature/change to test
- Business goal
- Current baseline metrics
- Available traffic

### Constraints
- Timeline requirements
- Technical limitations
- Risk tolerance

## Output Format

```markdown
# A/B Test Specification: [Test Name]

## Overview
**Feature Area:** [Where in game]
**Test Type:** [UI/Feature/Monetization/etc.]
**Priority:** [P0/P1/P2]
**Status:** [Draft/Approved/Running/Complete]

## Hypothesis

### Problem Statement
[What problem are we trying to solve?]

### Hypothesis
We believe that **[change]**
will result in **[primary metric] improving by [X]%**
because **[reasoning based on data/research]**

### Expected Outcome
- Primary metric: +[X]% ([confidence level])
- Secondary metric: +/- [Y]%

## Test Design

### Control (A)
**Name:** [Descriptive name]
**Description:** [Current experience]
**Traffic:** [%]

### Treatment (B)
**Name:** [Descriptive name]
**Description:** [Changed experience]
**Changes:**
- [Change 1]
- [Change 2]
**Traffic:** [%]

### [Treatment (C) if applicable]
[Same structure]

## Metrics

### Primary Metric
**Metric:** [Exact metric name]
**Current Baseline:** [Value]
**Minimum Detectable Effect (MDE):** [% change]
**Target:** [Absolute value or % improvement]

### Secondary Metrics
| Metric | Type | Current | Watch For |
|--------|------|---------|-----------|
| [Metric] | Guardrail | [Value] | Decrease > [X]% |
| [Metric] | Directional | [Value] | Increase expected |
| [Metric] | Diagnostic | [Value] | Explains results |

### Guardrail Metrics
| Metric | Threshold | Action if Violated |
|--------|-----------|-------------------|
| [Metric] | -[X]% | Stop test |
| [Metric] | -[Y]% | Investigate |

## Statistical Design

### Sample Size
**Baseline Rate:** [%]
**MDE:** [%] relative / [abs] absolute
**Statistical Significance:** 95% (p < 0.05)
**Statistical Power:** 80%
**Required Sample:** [N] per variant
**Total Required:** [N × variants]

### Duration
**Daily Eligible Users:** [N]
**Minimum Duration:** [X days]
**Maximum Duration:** [Y days]
**Planned Duration:** [Z days]

### Randomization
**Unit:** [User/Session/Device]
**Method:** [Hash-based/Random assignment]
**Stickiness:** [User stays in variant for duration]

## Segments

### Pre-Planned Segments
| Segment | Why | Hypothesis |
|---------|-----|------------|
| New vs Returning | [Reason] | [Expected difference] |
| Platform | [Reason] | [Expected difference] |
| Region | [Reason] | [Expected difference] |

### Exclusions
- [Exclusion criteria and reason]

## Implementation

### Technical Requirements
- [ ] [Requirement 1]
- [ ] [Requirement 2]

### Analytics Events
| Event | Parameters | Purpose |
|-------|------------|---------|
| [Event] | [Params] | [Why needed] |

### Feature Flags
**Flag Name:** [name]
**Configuration:** [Details]

## Rollout Plan

### Timeline
| Phase | Date | Traffic | Action |
|-------|------|---------|--------|
| Setup | [Date] | 0% | Deploy code |
| Internal | [Date] | Internal | Team testing |
| Soft launch | [Date] | [X]% | Initial rollout |
| Full test | [Date] | 50/50 | Full traffic |
| Analysis | [Date] | Hold | Review results |
| Decision | [Date] | - | Ship or revert |

### Monitoring
- Daily check: [Metrics to monitor]
- Alert threshold: [When to escalate]
- Owner: [Name]

## Decision Framework

### Success Criteria
- [ ] Primary metric improves by ≥ [X]% with p < 0.05
- [ ] [Guardrail 1] does not decrease by > [Y]%
- [ ] [Guardrail 2] does not decrease by > [Z]%

### Decision Matrix
| Primary Result | Guardrails | Decision |
|----------------|------------|----------|
| Significant win | Pass | Ship to 100% |
| Significant win | Fail | Investigate, likely revert |
| Not significant | Pass | [Specific decision] |
| Significant loss | Any | Revert |

## Risks

| Risk | Likelihood | Impact | Mitigation |
|------|------------|--------|------------|
| [Risk] | [H/M/L] | [H/M/L] | [Plan] |

## Documentation

### Pre-Test
- [ ] Hypothesis documented
- [ ] Metrics defined
- [ ] Sample size calculated
- [ ] Implementation complete
- [ ] QA approved

### Post-Test
- [ ] Results documented
- [ ] Learnings captured
- [ ] Follow-up tests identified
- [ ] Knowledge shared
```

Generate the test specification based on the context provided.
