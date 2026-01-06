---
name: a11y-check
description: Quick accessibility scan of a game feature - identify barriers and get immediate recommendations
---

# Quick Accessibility Check

Rapid accessibility scan of a specific feature, screen, or mechanic.

## Process

1. Identify what to check
2. Scan all four accessibility pillars
3. Identify top barriers
4. Provide quick fixes
5. Note platform-specific concerns

## Output Format

```markdown
## A11y Check: [Feature/Screen]

### Quick Assessment
**Risk Level:** [High/Medium/Low]
**Biggest Barrier:** [Most significant accessibility issue]

### Pillar Scan

| Pillar | Status | Key Issue |
|--------|--------|-----------|
| Visual | [OK/Warning/Fail] | [Issue or "None"] |
| Motor | [OK/Warning/Fail] | [Issue or "None"] |
| Cognitive | [OK/Warning/Fail] | [Issue or "None"] |
| Auditory | [OK/Warning/Fail] | [Issue or "None"] |

### Barriers Found

1. **[Barrier]:** Affects [who], [severity]
2. **[Barrier]:** Affects [who], [severity]
3. **[Barrier]:** Affects [who], [severity]

### Quick Fixes

| Issue | Fix | Effort |
|-------|-----|--------|
| [Issue] | [Solution] | [Low/Med] |
| [Issue] | [Solution] | [Low/Med] |
| [Issue] | [Solution] | [Low/Med] |

### Platform Flags
[Any platform certification concerns]

### Check These
- [ ] Color contrast meets 4.5:1 for text
- [ ] Controls can be remapped
- [ ] Audio has visual alternative
- [ ] Text is readable at minimum size
```

## Quick Questions

If context is missing, ask:
- "What screen or feature should I check?"
- "What platforms are you targeting?"
- "What accessibility features exist already?"
