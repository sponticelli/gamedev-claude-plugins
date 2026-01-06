---
name: scope-report
description: Full scope drift analysis with metrics - comprehensive audit of project scope health
---

# Scope Health Report

Generate a comprehensive scope analysis for a project or milestone.

## Process

1. Gather project information (pillars, original scope, current scope)
2. Calculate scope drift metrics
3. Identify scope creep patterns
4. Evaluate each major feature against pillars
5. Generate health score and recommendations

## Required Information

Ask the user for:
- Design pillars (3-5)
- Original planned features/scope
- Current features/scope
- Time remaining vs. time elapsed
- Any features added since planning

## Output Format

```markdown
# Scope Health Report: [Project Name]

## Executive Summary
**Scope Drift:** [X%] | **Health Score:** [X/10] | **Risk Level:** [Low/Medium/High/Critical]

[2-3 sentence summary of findings]

---

## Design Pillars
1. **[Pillar 1]:** [Description]
2. **[Pillar 2]:** [Description]
3. **[Pillar 3]:** [Description]

---

## Scope Metrics

### Feature Count
| Metric | Count |
|--------|-------|
| Originally Planned | [#] |
| Currently In Scope | [#] |
| Added Since Planning | [#] |
| Cut Since Planning | [#] |
| Net Change | [+/-#] |

### Scope Drift Calculation
```
([Current] - [Original]) / [Original] × 100 = [X%] drift
```

### Drift Assessment
- 0-10%: Healthy iteration
- 10-25%: Caution zone
- 25-50%: Scope review urgent
- 50%+: Project redefinition needed

**Your Status:** [Assessment]

---

## Feature-Pillar Matrix

| Feature | P1 | P2 | P3 | Score | Status |
|---------|----|----|----| ------|--------|
| [Feature 1] | [Y/N/P] | [Y/N/P] | [Y/N/P] | [X/3] | [Core/At Risk/Cut] |
| [Feature 2] | [Y/N/P] | [Y/N/P] | [Y/N/P] | [X/3] | [Core/At Risk/Cut] |
...

**Legend:** Y=Yes, N=No, P=Partial

---

## Scope Creep Patterns Detected

### [Pattern Name] - [Severity: Low/Med/High]
**Evidence:** [What triggered this detection]
**Impact:** [How it's affecting the project]
**Recommendation:** [How to address]

[Repeat for each detected pattern]

---

## Risk Assessment

| Risk | Likelihood | Impact | Urgency |
|------|------------|--------|---------|
| Deadline miss due to scope | [H/M/L] | [H/M/L] | [Immediate/Soon/Monitor] |
| Quality compromise | [H/M/L] | [H/M/L] | [Immediate/Soon/Monitor] |
| Team burnout | [H/M/L] | [H/M/L] | [Immediate/Soon/Monitor] |
| Vision dilution | [H/M/L] | [H/M/L] | [Immediate/Soon/Monitor] |

---

## Recommendations

### Immediate Actions (This Week)
1. [Specific action with owner]
2. [Specific action with owner]

### Cut List (Suggested)
| Feature | Reason | Savings |
|---------|--------|---------|
| [Feature] | [Why cut] | [Time/effort saved] |

### Reduce List (Scope Down)
| Feature | Current Scope | Reduced Scope | Savings |
|---------|---------------|---------------|---------|
| [Feature] | [Current] | [Smaller version] | [Time saved] |

### Defer List (Post-Launch)
| Feature | Reason to Defer | Notes |
|---------|-----------------|-------|
| [Feature] | [Why later is fine] | [Any context] |

---

## Scope Health Score: [X/10]

### Scoring Breakdown
| Factor | Score | Notes |
|--------|-------|-------|
| Pillar alignment | [X/10] | [Comment] |
| Feature discipline | [X/10] | [Comment] |
| Drift management | [X/10] | [Comment] |
| Risk awareness | [X/10] | [Comment] |

### Trend
[Improving / Stable / Declining] since last review

---

## Action Plan

| Priority | Action | Owner | Deadline |
|----------|--------|-------|----------|
| 1 | [Most urgent action] | [Who] | [When] |
| 2 | [Second action] | [Who] | [When] |
| 3 | [Third action] | [Who] | [When] |

---

*Report generated for scope review. Next review recommended: [Date/Milestone]*
```

## Guidelines

- Be honest about scope problems - sugar-coating helps no one
- Every cut suggestion should include reasoning
- Focus on what serves the pillars, not what's "cool"
- Consider team morale when recommending cuts
- Offer smaller versions before full cuts where possible
