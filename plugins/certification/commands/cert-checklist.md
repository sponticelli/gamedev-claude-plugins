---
name: cert-checklist
description: Generate a platform-specific certification requirements checklist
---

# Certification Checklist Generator

Create a certification requirements checklist for a specific platform.

## Context Gathering

Before generating the checklist, understand the context:

### Identify Platform
- Which platform is this for?
- What's the current TRC/XR version?
- Regional variations?
- Special programs (indie, Game Pass, etc.)?

### Understand Game Features
- What features does the game have?
- Online or offline only?
- Multiplayer modes?
- User-generated content?
- In-app purchases?

### Check Project Status
- Where in development?
- What's already been tested?
- Known problem areas?
- Previous certification experience?

### Identify Scope
- First submission or update?
- Full checklist or focused areas?
- All features or specific subset?

Use this context to create relevant checklist.

## Output Format

```markdown
# Certification Checklist: [Platform Name]

## Overview
**Platform:** [Platform]
**TRC/XR version:** [Version]
**Game features:** [Key features affecting cert]
**Last updated:** [Date]

## Quick Reference

### Legend
- [ ] Not tested
- [x] Passed
- [!] Failed (needs fix)
- [~] Waiver requested
- [N/A] Not applicable

### Priority
- **P0** - Blocking, must pass
- **P1** - High priority, likely blocking
- **P2** - Medium priority
- **P3** - Low priority

## System Requirements

### Boot & Initialization [P0]
- [ ] Game boots without error
- [ ] Loading screens display correctly
- [ ] No debug/placeholder text visible
- [ ] EULA/Terms display on first boot
- [ ] Region-appropriate content on start

### Save System [P0]
- [ ] Auto-save functions correctly
- [ ] Manual save available and works
- [ ] Save corruption handled gracefully
- [ ] Full storage handled appropriately
- [ ] Save data validated on load
- [ ] Progress saves to correct user

### Suspend/Resume [P0]
- [ ] Quick resume works correctly
- [ ] State preserved accurately
- [ ] Audio resumes correctly
- [ ] Network reconnects appropriately
- [ ] Controller reconnects

## User Management

### Account Handling [P0]
- [ ] Sign-in required at appropriate times
- [ ] Sign-out handled gracefully
- [ ] Profile switch handled
- [ ] Guest accounts work correctly
- [ ] Multiple user support

### Privacy [P1]
- [ ] Privacy settings respected
- [ ] Data collection disclosed
- [ ] Parental controls work
- [ ] COPPA compliance (if applicable)

## Input & Controllers

### Controller Support [P0]
- [ ] All required controllers work
- [ ] Button prompts correct for controller
- [ ] Prompts update when controller changes
- [ ] All actions achievable with controller

### Controller States [P0]
- [ ] Disconnect during gameplay
- [ ] Disconnect during save
- [ ] Reconnect handling
- [ ] Low battery handling

### Accessibility [P1]
- [ ] Button remapping available
- [ ] Colorblind options (if applicable)
- [ ] Text size options (if applicable)
- [ ] Required accessibility features

## Network Features

### Connectivity [P0]
- [ ] Offline mode available (if applicable)
- [ ] Connection loss handled
- [ ] Reconnection works
- [ ] Timeout handling
- [ ] NAT type handling

### Online Features [P0]
- [ ] Friends list integration
- [ ] Matchmaking functions
- [ ] Voice chat (if applicable)
- [ ] Content sharing (if applicable)
- [ ] Leaderboards (if applicable)

### Commerce [P0]
- [ ] IAP functions correctly
- [ ] Purchase flow compliant
- [ ] Restore purchases works
- [ ] Price display correct
- [ ] Transaction failures handled

## Platform Features

### Achievements/Trophies [P1]
- [ ] All achievements obtainable
- [ ] Unlock conditions correct
- [ ] Hidden achievements appropriate
- [ ] Points/grades comply

### Cloud Features [P1]
- [ ] Cloud save works
- [ ] Conflict resolution
- [ ] Sync status indicated
- [ ] Offline play syncs later

### Platform Integration [P2]
- [ ] Share/streaming features
- [ ] Activity feeds (if applicable)
- [ ] Platform-specific features

## Content & Ratings

### Age Rating [P0]
- [ ] Rating accurate
- [ ] Content descriptors accurate
- [ ] No undisclosed content
- [ ] Regional requirements met

### Localization [P1]
- [ ] All required languages present
- [ ] Text fits in UI
- [ ] No truncation
- [ ] Localized prompts

## Performance

### Technical [P0]
- [ ] Frame rate requirements met
- [ ] Load time requirements met
- [ ] No crashes after extended play
- [ ] Memory requirements met

### Stability [P0]
- [ ] 8+ hour soak test passed
- [ ] Stress test passed
- [ ] No reproducible crashes
- [ ] No soft locks

## Issue Tracking

| ID | Severity | Description | Status |
|----|----------|-------------|--------|
| | | | |

## Notes
[Additional notes and observations]
```

Generate based on the user's platform and game requirements.
