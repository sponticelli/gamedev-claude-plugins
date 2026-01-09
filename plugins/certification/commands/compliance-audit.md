---
name: compliance-audit
description: Perform a compliance audit against platform requirements
---

# Compliance Audit Generator

Create a compliance audit report against platform requirements.

## Context Gathering

Before generating the audit, understand the context:

### Identify Scope
- Which platform requirements?
- Full audit or specific areas?
- Current build version?
- Previous audit results?

### Understand Current State
- What's been tested?
- Known issues?
- Recent changes?
- Fix verification needed?

### Check Resources
- Test hardware available?
- Test accounts set up?
- Documentation accessible?
- Time allocation?

### Identify Focus Areas
- High-risk features?
- Previously failed areas?
- New features since last audit?
- Regression testing needed?

Use this context to create focused audit.

## Output Format

```markdown
# Compliance Audit Report

## Audit Information
**Platform:** [Platform name]
**Requirements version:** [TRC/XR version]
**Build tested:** [Build number]
**Test date:** [Date]
**Auditor:** [Name]
**Scope:** [Full/Focused on X]

## Executive Summary

**Recommendation:** [Ready/Not ready for submission]

| Category | Pass | Fail | Waiverable | N/A |
|----------|------|------|------------|-----|
| System | [N] | [N] | [N] | [N] |
| Input | [N] | [N] | [N] | [N] |
| Network | [N] | [N] | [N] | [N] |
| Platform | [N] | [N] | [N] | [N] |
| Content | [N] | [N] | [N] | [N] |
| **Total** | **[N]** | **[N]** | **[N]** | **[N]** |

## Blocking Issues

### [Issue ID]: [Issue Title]
**Requirement:** [TRC/XR number]
**Severity:** [Critical/Major]
**Category:** [System/Input/Network/etc.]

**Description:**
[What the issue is]

**Steps to Reproduce:**
1. [Step 1]
2. [Step 2]
3. [Step 3]

**Expected Result:**
[What should happen]

**Actual Result:**
[What happens]

**Evidence:**
[Screenshot/video reference]

**Recommendation:**
[How to fix]

---

[Repeat for each blocking issue]

## Non-Blocking Issues

### [Issue ID]: [Issue Title]
**Requirement:** [TRC/XR number]
**Severity:** [Minor]
**Waiverable:** [Yes/No/Maybe]

**Description:**
[Brief description]

**Waiver justification (if applicable):**
[Why this could be waived]

---

[Repeat for each non-blocking issue]

## Passed Areas

### System Features
| Test | Result | Notes |
|------|--------|-------|
| [Test case] | Pass | [Any notes] |

### Input/Controller
| Test | Result | Notes |
|------|--------|-------|
| [Test case] | Pass | [Any notes] |

### Network
| Test | Result | Notes |
|------|--------|-------|
| [Test case] | Pass | [Any notes] |

### Platform Features
| Test | Result | Notes |
|------|--------|-------|
| [Test case] | Pass | [Any notes] |

### Content
| Test | Result | Notes |
|------|--------|-------|
| [Test case] | Pass | [Any notes] |

## Not Tested

| Area | Reason |
|------|--------|
| [Area] | [Why not tested] |

## Recommendations

### Before Submission
1. [Must fix issue 1]
2. [Must fix issue 2]

### Should Fix If Time Allows
1. [Issue 1]
2. [Issue 2]

### Future Considerations
1. [Suggestion 1]
2. [Suggestion 2]

## Test Environment

| Parameter | Value |
|-----------|-------|
| Hardware | [Model] |
| Firmware | [Version] |
| SDK | [Version] |
| Region | [Region] |
| Language | [Languages tested] |

## Appendix

### Test Cases Executed
[Full list of test cases run]

### Evidence Archive
[Location of screenshots/videos]
```

Generate based on the user's platform and audit requirements.
