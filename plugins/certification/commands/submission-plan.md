---
name: submission-plan
description: Generate a certification submission timeline and plan
---

# Submission Plan Generator

Create a certification submission timeline and plan.

## Context Gathering

Before generating the submission plan, understand the project:

### Identify Targets
- Which platforms?
- Target release date?
- Simultaneous or staggered release?
- Day-one patch strategy?

### Understand Current State
- Development phase?
- Content complete?
- Known blockers?
- Previous certification experience?

### Check Resources
- Who handles submissions?
- Testing capacity?
- Platform relationships?
- Budget for certification?

### Identify Constraints
- Hard deadlines?
- Marketing commitments?
- Platform launch windows?
- Regional requirements?

Use this context to create realistic plan.

## Output Format

```markdown
# Submission Plan: [Game Title]

## Overview
**Target release:** [Date]
**Platforms:** [List with priority]
**Submission lead:** [Name]
**Strategy:** [Simultaneous/Staggered]

## Platform Summary

| Platform | Target Submit | Expected Result | Release |
|----------|---------------|-----------------|---------|
| [Platform] | [Date] | [Date] | [Date] |

## Timeline

### Visual Timeline
```
Week -8  -7  -6  -5  -4  -3  -2  -1   0
  │   │   │   │   │   │   │   │   │
  │   │   │   │   └─Submission────│
  │   │   │   │                   │
  │   │   └─Final fixes───────────│
  │   │                           │
  └─Internal cert testing─────────│
                                  │
                              RELEASE
```

### Detailed Timeline

#### [Platform 1]
| Milestone | Date | Owner | Deliverables |
|-----------|------|-------|--------------|
| Code complete | [Date] | [Who] | Final build |
| Content complete | [Date] | [Who] | All assets |
| Internal cert 1 | [Date] | [Who] | Test report |
| Fix period | [Date-Date] | [Who] | Bug fixes |
| Internal cert 2 | [Date] | [Who] | Verification |
| Prepare submission | [Date] | [Who] | Package ready |
| Submit | [Date] | [Who] | Submitted |
| Review period | [Date-Date] | - | Awaiting result |
| Response window | [Date-Date] | [Who] | Handle feedback |
| Expected pass | [Date] | - | Certification |
| Resubmit buffer | [Date] | [Who] | If needed |
| Release | [Date] | [Who] | Launch |

[Repeat for each platform]

## Submission Package Preparation

### Build Requirements
| Item | Status | Owner | Due |
|------|--------|-------|-----|
| Final build | [Status] | [Who] | [Date] |
| Build notes | [Status] | [Who] | [Date] |
| Known issues doc | [Status] | [Who] | [Date] |
| Test credentials | [Status] | [Who] | [Date] |

### Documentation
| Document | Status | Owner | Due |
|----------|--------|-------|-----|
| Game description | [Status] | [Who] | [Date] |
| Feature list | [Status] | [Who] | [Date] |
| Network features | [Status] | [Who] | [Date] |
| Privacy policy | [Status] | [Who] | [Date] |

### Assets
| Asset | Status | Owner | Due |
|-------|--------|-------|-----|
| Store icons | [Status] | [Who] | [Date] |
| Screenshots | [Status] | [Who] | [Date] |
| Trailer | [Status] | [Who] | [Date] |
| Key art | [Status] | [Who] | [Date] |

## Risk Assessment

| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|------------|
| Save system issues | [H/M/L] | [H/M/L] | [Action] |
| Network failures | [H/M/L] | [H/M/L] | [Action] |
| Late content | [H/M/L] | [H/M/L] | [Action] |
| Platform delays | [H/M/L] | [H/M/L] | [Action] |

## Contingency Plans

### If First Submission Fails
**Available time:** [Days for resubmit]
**Priority process:** [How to fast-track fixes]
**Resubmission target:** [Date]

### If Multiple Resubmissions Needed
**Impact on release:** [What changes]
**Communication plan:** [How to handle]
**Maximum delay:** [How late can we go]

## Team Responsibilities

| Role | Person | Responsibilities |
|------|--------|------------------|
| Submission lead | [Name] | Overall coordination |
| QA lead | [Name] | Testing, bug triage |
| Dev lead | [Name] | Fix implementation |
| Producer | [Name] | Stakeholder comms |
| Platform contact | [Name] | Platform relationship |

## Communication Plan

### Internal Updates
- Daily standups during cert period
- Issue tracker for all cert bugs
- Slack channel for cert team

### External Updates
- Platform: [How/when to communicate]
- Publisher: [How/when to update]
- Marketing: [Launch readiness updates]

## Success Criteria

### For Submission
- [ ] All blockers fixed
- [ ] Internal cert passed
- [ ] All materials ready
- [ ] Team available for response

### For Launch
- [ ] Certification passed
- [ ] Day-one patch ready (if applicable)
- [ ] Store pages live
- [ ] Marketing aligned
```

Generate based on the user's project and submission requirements.
