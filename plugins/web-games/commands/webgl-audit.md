---
name: webgl-audit
description: Audit WebGL implementation for compatibility and performance
---

# WebGL Audit

Review WebGL implementation for compatibility, performance, and best practices.

## Audit Checklist

### Compatibility
- [ ] WebGL context creation handles failure
- [ ] Context loss recovery implemented
- [ ] Required extensions checked before use
- [ ] WebGL2 with WebGL1 fallback (if needed)
- [ ] Shader precision qualifiers appropriate

### Performance
- [ ] Draw calls per frame reasonable (< 200 ideal)
- [ ] State changes minimized
- [ ] Textures are power-of-two or handled
- [ ] No synchronous API calls in render loop
- [ ] Geometry batched appropriately

### Memory
- [ ] Texture memory budget defined
- [ ] Unused resources cleaned up
- [ ] No texture leaks
- [ ] Buffer reuse where possible

## Output Format

```markdown
# WebGL Audit Report: [Project Name]

## Summary
**WebGL Version:** [1.0/2.0]
**Health Score:** [X/10]
**Critical Issues:** [N]

## Compatibility Analysis
| Browser | Version | Status | Notes |
|---------|---------|--------|-------|
| Chrome | Latest | [Pass/Warn/Fail] | |
| Firefox | Latest | [Pass/Warn/Fail] | |
| Safari | Latest | [Pass/Warn/Fail] | |
| iOS Safari | Latest | [Pass/Warn/Fail] | |
| Android Chrome | Latest | [Pass/Warn/Fail] | |

## Extension Requirements
| Extension | Required | Fallback Available | Status |
|-----------|----------|-------------------|--------|
| [Extension] | [Yes/Optional] | [Yes/No] | [✓/✗] |

## Performance Metrics
| Metric | Current | Target | Status |
|--------|---------|--------|--------|
| Draw calls/frame | [N] | < 200 | [✓/✗] |
| Triangles/frame | [N] | < 100K | [✓/✗] |
| State changes | [N] | < 50 | [✓/✗] |
| Texture memory | [MB] | < 256MB | [✓/✗] |

## Issues Found

### Critical
| Issue | Location | Impact | Fix |
|-------|----------|--------|-----|
| [Issue] | [File:Line] | [Severity] | [Solution] |

### Warnings
| Issue | Location | Impact | Fix |
|-------|----------|--------|-----|
| [Issue] | [File:Line] | [Severity] | [Solution] |

## Shader Analysis
| Shader | Complexity | Mobile Safe | Issues |
|--------|------------|-------------|--------|
| [Name] | [Low/Med/High] | [Yes/No] | [Issues] |

## Recommendations
1. [Priority 1 recommendation]
2. [Priority 2 recommendation]
3. [Priority 3 recommendation]
```

Analyze the WebGL implementation and provide actionable feedback.
