---
name: code-review
description: Quick code review focused on game development best practices - catches common issues and suggests improvements
---

# Game Code Review

Review the provided code with game development specific concerns.

## Review Checklist

### Performance
- [ ] Hot path optimizations (update loops, physics callbacks)
- [ ] Allocation in update (GC pressure)
- [ ] Cache-unfriendly access patterns
- [ ] Unnecessary component lookups
- [ ] Missing object pooling for frequent spawns

### Game-Specific
- [ ] Frame-rate independent movement (delta time)
- [ ] Input handling best practices
- [ ] State machine structure
- [ ] Event subscription cleanup
- [ ] Save/load considerations

### Architecture
- [ ] Clear responsibilities
- [ ] Appropriate coupling
- [ ] Testability
- [ ] Debugging support

### Common Bugs
- [ ] Null reference potential
- [ ] Off-by-one errors
- [ ] Race conditions
- [ ] Order of operations

## Output Format

```markdown
## Code Review: [File/Feature]

### Summary
[One paragraph overview of the code and its quality]

### Issues Found

#### 🔴 Critical
[Bugs or performance issues that need immediate attention]

#### 🟡 Improvements
[Suggested enhancements for code quality]

#### 🟢 Nice-to-Have
[Minor polish suggestions]

### Positive Notes
[What's done well - be specific]

### Suggested Refactors
[If substantial changes would help, describe them]
```

Review the code the user provides.
