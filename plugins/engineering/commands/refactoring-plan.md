---
name: refactoring-plan
description: Create a structured approach for code refactoring
---

# Refactoring Plan Generator

Create a systematic plan for refactoring code safely and effectively.

## Context Gathering

Before planning the refactoring, understand the situation:

### Identify the Problem
- What's wrong with the current code?
- What pain does it cause?
- How often does it cause problems?
- What's the business impact?

### Understand the Code
- What does this code do?
- How old is it?
- Who knows it best?
- What depends on it?

### Assess Risk
- How critical is this code?
- What's the test coverage?
- What could break?
- What's the rollback strategy?

### Define Success
- What does "done" look like?
- How will you know it worked?
- What metrics improve?
- What's acceptable downtime/risk?

Use this context to create an appropriate refactoring plan.

## Output Format

```markdown
# Refactoring Plan: [Component/System Name]

## Overview

### Current State
**What exists:**
[Brief description of current implementation]

**Problems:**
| Problem | Impact | Frequency |
|---------|--------|-----------|
| [Issue] | [Effect on team/product] | [How often] |

**Code location:**
- Primary: `[path/to/main/file.ext]`
- Related: `[other/files.ext]`

### Target State
**What we want:**
[Description of desired outcome]

**Benefits:**
| Benefit | Value | Measurement |
|---------|-------|-------------|
| [Benefit] | [Why it matters] | [How to verify] |

### Scope
**In scope:**
- [What will change]
- [What will change]

**Out of scope:**
- [What we're explicitly NOT touching]
- [What we're explicitly NOT touching]

---

## Risk Assessment

### Code Criticality
**Business impact if broken:** [Critical / High / Medium / Low]
**User-facing:** [Yes / No]
**Data sensitivity:** [Handles sensitive data / No]

### Test Coverage
**Current coverage:**
- Unit tests: [Yes/No, %]
- Integration tests: [Yes/No, %]
- E2E tests: [Yes/No]

**Coverage gaps:**
- [Area without tests]
- [Area without tests]

### Dependencies
**What depends on this code:**
| Dependent | How it uses this code |
|-----------|----------------------|
| [Module/Service] | [Usage pattern] |

**What this code depends on:**
| Dependency | Concern |
|------------|---------|
| [Module/Service] | [Stability concern] |

### Risk Level
**Overall risk:** [High / Medium / Low]
**Rationale:** [Why this risk level]

---

## Preparation

### Before Starting

#### Documentation
- [ ] Document current behavior
- [ ] Map dependencies
- [ ] Note undocumented behaviors
- [ ] Identify edge cases

#### Testing Foundation
- [ ] Achieve minimum test coverage for affected areas
- [ ] Add characterization tests for unclear behavior
- [ ] Verify tests pass in CI
- [ ] Set up test environment if needed

#### Safety Nets
- [ ] Feature flag available (if applicable)
- [ ] Rollback plan documented
- [ ] Monitoring in place
- [ ] Team aligned on plan

### Required Before Proceeding
| Requirement | Status | Owner |
|-------------|--------|-------|
| [Requirement] | [Done/Pending] | [Who] |

---

## Refactoring Strategy

### Approach
**Strategy:** [Strangler Fig / Branch by Abstraction / Parallel Change / Big Bang]

**Rationale:**
[Why this approach fits]

### Phases

#### Phase 1: [Name]
**Goal:** [What this phase achieves]
**Duration estimate:** [Not a timeline, but relative size: small/medium/large]

**Steps:**
1. [Specific action]
2. [Specific action]
3. [Specific action]

**Checkpoint:**
- [ ] [Verification that phase is complete]
- [ ] Tests pass
- [ ] No regressions

#### Phase 2: [Name]
**Goal:** [What this phase achieves]
**Depends on:** Phase 1 completion

**Steps:**
1. [Specific action]
2. [Specific action]
3. [Specific action]

**Checkpoint:**
- [ ] [Verification that phase is complete]
- [ ] Tests pass
- [ ] No regressions

[Continue for additional phases]

#### Final Phase: Cleanup
**Goal:** Remove old code and technical debt

**Steps:**
1. Remove deprecated code paths
2. Remove feature flags (if used)
3. Update documentation
4. Archive/delete old implementations

**Checkpoint:**
- [ ] No dead code remains
- [ ] Documentation updated
- [ ] Team informed

---

## Technical Approach

### Patterns to Apply
| Pattern | Where | Why |
|---------|-------|-----|
| [Pattern] | [Location] | [Benefit] |

### Principles to Follow
- [ ] Keep commits small and atomic
- [ ] Each commit leaves code working
- [ ] Separate refactoring commits from behavior changes
- [ ] No big bang changes without tests

### Code Standards
**Apply these standards during refactoring:**
- [Standard 1]
- [Standard 2]
- [Standard 3]

### Techniques
**Primary refactoring techniques:**
| Technique | Use Case |
|-----------|----------|
| Extract Method | [When to use] |
| Inline | [When to use] |
| Rename | [When to use] |
| Move | [When to use] |
| [Other] | [When to use] |

---

## Testing Strategy

### Before Each Change
- [ ] Tests pass
- [ ] Change is understood

### During Refactoring
- [ ] Run tests after each small change
- [ ] Add tests for discovered edge cases
- [ ] Document surprising behaviors

### Test Types
| Test Type | Purpose | When to Run |
|-----------|---------|-------------|
| Unit | Verify functions work | Every save/commit |
| Integration | Verify components work together | Before push |
| E2E | Verify user flows | Before merge |

### New Tests Needed
| Area | Test Type | Description |
|------|-----------|-------------|
| [Area] | [Type] | [What to test] |

---

## Rollback Plan

### If Things Go Wrong

#### Minor Issues
**Symptoms:** Tests fail, but easy to fix
**Action:** Fix forward, don't merge until green

#### Medium Issues
**Symptoms:** Unexpected behavior in staging
**Action:** Revert PR, investigate, re-plan

#### Critical Issues
**Symptoms:** Production incident
**Action:**
1. Revert immediately
2. Confirm stability
3. Investigate root cause
4. Update plan before retry

### Revert Commands
```bash
# Revert last merge
git revert -m 1 [merge-commit-hash]

# If using feature flag
[command to disable flag]

# Database rollback (if applicable)
[migration rollback command]
```

### Data Considerations
**Database changes:** [Yes/No]
**Reversible:** [Yes/No]
**Data migration plan:** [If applicable]

---

## Validation

### Definition of Done
- [ ] All tests pass
- [ ] Code review approved
- [ ] No performance regression
- [ ] Documentation updated
- [ ] Team walkthrough complete (if significant)

### Performance Validation
**Benchmarks:**
| Metric | Before | Target | After |
|--------|--------|--------|-------|
| [Metric] | [Value] | [Value] | [TBD] |

### Quality Validation
**Static analysis:**
- [ ] No new warnings
- [ ] Complexity reduced (or not increased)
- [ ] Coverage maintained or improved

---

## Communication

### Stakeholders
| Who | What They Need to Know | When |
|-----|------------------------|------|
| [Team] | [Information] | [Timing] |

### Updates
- [ ] Kick-off: Inform team of plan
- [ ] Progress: Regular updates during work
- [ ] Completion: Summary of changes

### Documentation Updates
- [ ] Code comments
- [ ] README/docs
- [ ] Architecture docs
- [ ] Runbook (if applicable)

---

## Checklist Summary

### Pre-Flight
- [ ] Plan reviewed and approved
- [ ] Tests in place
- [ ] Team informed
- [ ] Rollback plan ready

### Per-Phase
- [ ] Changes committed atomically
- [ ] Tests pass after each change
- [ ] Code review for phase complete
- [ ] Checkpoint verified

### Completion
- [ ] All phases complete
- [ ] Old code removed
- [ ] Documentation updated
- [ ] Performance validated
- [ ] Team notified
```

Generate a refactoring plan appropriate for the complexity and risk level.
