---
name: a11y-plan
description: Full accessibility implementation plan - comprehensive roadmap for making a game accessible
---

# Accessibility Implementation Plan

Generate a complete accessibility roadmap for a game or major feature.

## Process

1. Gather game information (genre, platforms, current state)
2. Assess current accessibility level
3. Identify all gaps by pillar
4. Prioritize by impact and effort
5. Create phased implementation plan

## Required Information

Ask the user for:
- Game genre and core mechanics
- Target platforms
- Current accessibility features (if any)
- Timeline constraints
- Platform certification requirements

## Output Format

```markdown
# Accessibility Implementation Plan: [Game Name]

## Project Overview
**Genre:** [Genre]
**Platforms:** [List]
**Current A11y Level:** [None/Basic/Intermediate/Advanced]
**Target Level:** [Basic/Intermediate/Advanced/Exemplary]

---

## Gap Analysis

### Visual Accessibility
| Feature | Current State | Target | Gap |
|---------|---------------|--------|-----|
| Subtitles | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Text sizing | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Colorblind support | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| High contrast | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Screen reader | [Yes/No/Partial] | [Required/Recommended] | [Description] |

### Motor Accessibility
| Feature | Current State | Target | Gap |
|---------|---------------|--------|-----|
| Remapping | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Toggle options | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Timing adjustments | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| One-handed support | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Difficulty options | [Yes/No/Partial] | [Required/Recommended] | [Description] |

### Cognitive Accessibility
| Feature | Current State | Target | Gap |
|---------|---------------|--------|-----|
| Quest/objective log | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Tutorial replay | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Speed options | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Save system | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Clear language | [Yes/No/Partial] | [Required/Recommended] | [Description] |

### Auditory Accessibility
| Feature | Current State | Target | Gap |
|---------|---------------|--------|-----|
| Subtitles | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Closed captions | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Visual audio cues | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Volume controls | [Yes/No/Partial] | [Required/Recommended] | [Description] |
| Mono audio | [Yes/No/Partial] | [Required/Recommended] | [Description] |

---

## Platform Requirements

### [Platform 1]
**Certification Requirements:**
- [ ] [Requirement 1]
- [ ] [Requirement 2]
- [ ] [Requirement 3]

**Current Compliance:** [Pass/Fail/At Risk]
**Gaps to Close:** [List]

[Repeat for each platform]

---

## Implementation Phases

### Phase 1: Foundations (Critical Path)
**Goal:** Meet minimum requirements, address blocking issues

| Feature | Description | Effort | Owner |
|---------|-------------|--------|-------|
| [Feature] | [What to build] | [Days/Weeks] | [Team/Person] |

**Exit Criteria:** [What "done" looks like]

### Phase 2: Core Accessibility
**Goal:** Achieve solid baseline accessibility

| Feature | Description | Effort | Owner |
|---------|-------------|--------|-------|
| [Feature] | [What to build] | [Days/Weeks] | [Team/Person] |

**Exit Criteria:** [What "done" looks like]

### Phase 3: Enhanced Accessibility
**Goal:** Go beyond minimum, serve more players

| Feature | Description | Effort | Owner |
|---------|-------------|--------|-------|
| [Feature] | [What to build] | [Days/Weeks] | [Team/Person] |

**Exit Criteria:** [What "done" looks like]

### Phase 4: Polish & Excellence (If Time Allows)
**Goal:** Exemplary accessibility

| Feature | Description | Effort | Owner |
|---------|-------------|--------|-------|
| [Feature] | [What to build] | [Days/Weeks] | [Team/Person] |

---

## Technical Considerations

### Systems to Build
| System | Purpose | Dependencies |
|--------|---------|--------------|
| [System] | [What it enables] | [What it needs] |

### Integration Points
- [Where accessibility hooks into existing systems]

### Testing Requirements
- [How to test each feature]
- [Who should test (include disabled testers)]

---

## Accessibility Menu Design

```
Accessibility
├── Visual
│   ├── Subtitle Size [Small/Medium/Large/XL]
│   ├── Subtitle Background [Off/Dark/Solid]
│   ├── Colorblind Mode [Off/Protanopia/Deuteranopia/Tritanopia]
│   ├── High Contrast [Off/On]
│   └── UI Scale [80%/100%/120%/150%]
├── Audio
│   ├── Master Volume [Slider]
│   ├── Music Volume [Slider]
│   ├── SFX Volume [Slider]
│   ├── Voice Volume [Slider]
│   ├── Mono Audio [Off/On]
│   └── Visual Sound Indicators [Off/On]
├── Controls
│   ├── Button Remapping [→]
│   ├── Stick Sensitivity [Slider]
│   ├── Vibration [Off/Light/Full]
│   ├── Hold/Toggle Options [→]
│   └── Auto-Aim [Off/Light/Strong]
└── Gameplay
    ├── Difficulty [Options]
    ├── Game Speed [50%/75%/100%]
    ├── Extended Timers [Off/On]
    └── Auto-Skip QTEs [Off/On]
```

---

## Communication Plan

### In-Game
- First-run accessibility prompt
- Accessibility options always 1-2 taps away
- Context-sensitive tips

### Marketing
- Include accessibility in store descriptions
- Tag with accessibility features
- Create accessibility-focused media

---

## Success Metrics

| Metric | Target |
|--------|--------|
| Platform certification | [Pass all] |
| Basic features complete | [100%] |
| Player accessibility complaints | [<X per month] |
| Accessibility reviews positive | [Target] |

---

## Resources & References

- [Relevant guidelines links]
- [Tools to use]
- [Consultants/testers to engage]

---

*Plan created [Date]. Review at each milestone.*
```

## Guidelines

- Prioritize blocking issues first
- Phase work so game can ship at each phase
- Include disabled player testing in timeline
- Consider localization impact of text changes
- Document decisions for future reference
