---
name: postmortem
description: Structure a project or incident postmortem for learning and improvement
---

# Postmortem Generator

Create a structured postmortem document for projects, launches, or incidents.

## Context Gathering

Before creating the postmortem, gather relevant information:

### Check for Project Documentation
- Look for project plans, timelines, or milestone documents
- Review README or project overview files
- Check for existing retrospective notes or feedback
- Look for any previous postmortems for patterns

### Analyze Event Timeline
- Check git history to reconstruct sequence of events
- Look for deployment logs or release notes
- Review any issue tracker references (GitHub issues, etc.)
- Identify key dates and decision points

### Identify Stakeholders
- Who was involved in the project/incident
- Who was affected by the outcome
- Who can provide additional context or perspective
- Who should receive the postmortem findings

### Gather Metrics (if applicable)
- Look for analytics or monitoring data
- Check for error logs or crash reports
- Review any metrics dashboards or reports
- Note before/after comparisons where possible

Use this context to:
- Construct an accurate timeline
- Identify all contributing factors
- Ground lessons learned in specific evidence
- Ensure action items address actual root causes

## Output Format

```markdown
# Postmortem: [Subject]

## Summary
**Date:** [When]
**Type:** [Project/Launch/Incident]
**Severity:** [Critical/Major/Minor] (for incidents)
**Duration:** [How long]

### One-Sentence Summary
[What happened in one sentence]

## Timeline
| Time | Event |
|------|-------|
| [Time] | [What happened] |

## What Happened
[Detailed narrative of events]

## Impact
| Area | Impact | Measurement |
|------|--------|-------------|
| [Area] | [Description] | [Quantified] |

## Root Cause Analysis
### Contributing Factors
1. **[Factor 1]:** [Description]
2. **[Factor 2]:** [Description]
3. **[Factor 3]:** [Description]

### Root Cause
[The underlying issue that enabled this]

### 5 Whys Analysis
1. Why: [First answer]
2. Why: [Deeper answer]
3. Why: [Deeper still]
4. Why: [Getting to root]
5. Why: [Root cause]

## What Went Well
- [Positive 1]
- [Positive 2]
- [Positive 3]

## What Went Wrong
- [Issue 1]
- [Issue 2]
- [Issue 3]

## Lessons Learned
| Lesson | Category | Apply To |
|--------|----------|----------|
| [Lesson] | [Process/Tech/People] | [Future application] |

## Action Items
| Action | Owner | Due | Priority |
|--------|-------|-----|----------|
| [Action] | [Who] | [When] | [H/M/L] |

## Prevention Measures
[How to prevent this from happening again]

## Open Questions
[Things we still don't know]
```

## Postmortem Facilitation Notes

- **Blameless culture:** Focus on systems, not people
- **Honesty first:** Accurate timeline matters
- **Action-oriented:** Every lesson needs an action
- **Follow up:** Track action items to completion

Generate based on user's context.
