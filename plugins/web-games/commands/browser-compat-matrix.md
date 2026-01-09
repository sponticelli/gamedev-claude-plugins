---
name: browser-compat-matrix
description: Generate browser compatibility testing matrix
---

# Browser Compatibility Matrix Generator

Generate a comprehensive browser compatibility testing matrix for a web game.

## Context Gathering

Before generating, understand:

### Game Requirements
- Rendering (WebGL 1/2, Canvas 2D)
- Audio (Web Audio API)
- Input (Gamepad API, Touch)
- Storage (IndexedDB, localStorage)
- Other APIs used

### Target Audience
- Primary platforms
- Geographic regions
- Device categories

## Output Format

```markdown
# Browser Compatibility Matrix: [Game Name]

## Target Browser Support

### Tier 1: Full Support (Must Work)
| Browser | Version | Platform | Market Share |
|---------|---------|----------|--------------|
| Chrome | 90+ | Desktop | [%] |
| Chrome | 90+ | Android | [%] |
| Safari | 15+ | macOS | [%] |
| Safari | 15+ | iOS | [%] |
| Firefox | 90+ | Desktop | [%] |

### Tier 2: Basic Support (Should Work)
| Browser | Version | Platform | Market Share |
|---------|---------|----------|--------------|
| Edge | 90+ | Desktop | [%] |
| Samsung Internet | 15+ | Android | [%] |
| Chrome | 80-89 | All | [%] |

### Tier 3: Best Effort (May Work)
| Browser | Version | Notes |
|---------|---------|-------|
| [Browser] | [Version] | [Limitations] |

## Feature Compatibility

### Core Features
| Feature | Chrome | Firefox | Safari | Edge | Notes |
|---------|--------|---------|--------|------|-------|
| WebGL 2 | ✓ | ✓ | ✓* | ✓ | *iOS 15+ |
| WebGL 1 | ✓ | ✓ | ✓ | ✓ | Fallback |
| Canvas 2D | ✓ | ✓ | ✓ | ✓ | |
| Web Audio | ✓ | ✓ | ✓* | ✓ | *Gesture required |
| Gamepad API | ✓ | ✓ | ✓ | ✓ | |
| Touch Events | ✓ | ✓ | ✓ | ✓ | |
| Pointer Events | ✓ | ✓ | ✓ | ✓ | |

### Storage Features
| Feature | Chrome | Firefox | Safari | Edge | Notes |
|---------|--------|---------|--------|------|-------|
| IndexedDB | ✓ | ✓ | ✓* | ✓ | *Quota varies |
| localStorage | ✓ | ✓ | ✓ | ✓ | |
| Cache API | ✓ | ✓ | ✓ | ✓ | |

### PWA Features
| Feature | Chrome | Firefox | Safari | Edge | Notes |
|---------|--------|---------|--------|------|-------|
| Service Workers | ✓ | ✓ | ✓ | ✓ | |
| Add to Home | ✓ | ✗ | ✓* | ✓ | *Manual in Safari |
| Push Notifications | ✓ | ✓ | ✗ | ✓ | iOS: No push |
| Background Sync | ✓ | ✗ | ✗ | ✓ | |

### WebGL Extensions
| Extension | Chrome | Firefox | Safari | Notes |
|-----------|--------|---------|--------|-------|
| [Required ext] | [✓/✗] | [✓/✗] | [✓/✗] | [Usage] |
| [Optional ext] | [✓/✗] | [✓/✗] | [✓/✗] | [Fallback if ✗] |

## Test Matrix

### Desktop Testing
| Browser | OS | Resolution | Priority |
|---------|-----|------------|----------|
| Chrome latest | Windows 11 | 1920x1080 | P0 |
| Chrome latest | macOS | 1920x1080 | P0 |
| Firefox latest | Windows 11 | 1920x1080 | P0 |
| Safari latest | macOS | 1920x1080 | P0 |
| Edge latest | Windows 11 | 1920x1080 | P1 |

### Mobile Testing
| Browser | Device | OS Version | Priority |
|---------|--------|------------|----------|
| Safari | iPhone 13+ | iOS 16+ | P0 |
| Safari | iPad | iPadOS 16+ | P1 |
| Chrome | Pixel 6 | Android 12+ | P0 |
| Chrome | Galaxy S21 | Android 12+ | P1 |
| Samsung | Galaxy S21 | Android 12+ | P2 |

### Low-End Device Testing
| Device | Browser | Notes |
|--------|---------|-------|
| iPhone SE | Safari | Low resolution |
| Budget Android | Chrome | Limited GPU |
| 5-year-old PC | Chrome | Baseline desktop |

## Known Issues & Workarounds

### Safari/iOS
| Issue | Workaround |
|-------|------------|
| Audio requires gesture | Unlock on first tap |
| WebGL2 context attributes | Check support first |
| IndexedDB private mode | Detect and warn user |

### Firefox
| Issue | Workaround |
|-------|------------|
| [Issue] | [Workaround] |

### Mobile General
| Issue | Workaround |
|-------|------------|
| Orientation changes | Handle resize events |
| Virtual keyboard | Adjust viewport |
| Pull-to-refresh | Disable in manifest/CSS |

## Testing Checklist

### Per-Browser Tests
- [ ] Game loads without errors
- [ ] Rendering correct
- [ ] Audio plays
- [ ] Input responsive
- [ ] Save/load works
- [ ] Performance acceptable

### Cross-Browser Tests
- [ ] Consistent visual appearance
- [ ] Feature parity (where supported)
- [ ] Graceful degradation (where not)
- [ ] Error messages helpful

## Polyfills & Fallbacks
| Feature | Polyfill/Fallback | Size Impact |
|---------|-------------------|-------------|
| [Feature] | [Solution] | [KB] |
```

Generate the compatibility matrix based on the game requirements provided.
