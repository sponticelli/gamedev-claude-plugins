---
name: netcode-brief
description: Generate a low-level networking specification covering prediction, interpolation, and lag compensation
---

# Netcode Brief Generator

Create a detailed netcode specification for multiplayer game implementation.

## Context Gathering

Before generating the netcode brief, understand the networking needs:

### Analyze Game Mechanics
- What actions require instant feedback? (movement, shooting, abilities)
- What actions can tolerate latency? (inventory, chat, cosmetics)
- What's the tick rate / update frequency?
- Are there physics-based interactions?

### Understand Network Architecture
- Is this client-server or P2P?
- Who has authority over what?
- What's the expected latency range?
- What's the target bandwidth?

### Check Existing Netcode
- Is there existing networking code?
- What networking library/framework is used?
- Are there known sync issues to address?

### Identify Critical Systems
- What systems need prediction?
- What systems need interpolation?
- Is lag compensation needed for hit detection?

Use this context to design appropriate netcode techniques.

## Output Format

```markdown
# Netcode Specification: [Game/Feature]

## Overview
**Tick Rate:** [Server Hz]
**Update Rate:** [Client snapshot rate Hz]
**Latency Target:** [Xms RTT acceptable]
**Bandwidth Budget:** [X KB/s per player]

## Techniques

### Client-Side Prediction
**Applied to:**
- [System 1]: [How predicted]
- [System 2]: [How predicted]

**Not predicted (server-authoritative):**
- [System]: [Why not predicted]

**Reconciliation approach:**
[How server corrections are applied]

### Entity Interpolation
**Buffer size:** [X ms / Y updates]
**Interpolation method:** [Linear / Hermite / Custom]

**Per-entity settings:**
| Entity Type | Buffer | Priority |
|-------------|--------|----------|
| [Type] | [Xms] | [High/Med/Low] |

### Lag Compensation
**Enabled for:** [Systems]
**Max rewind:** [Xms]
**Validation:** [Server-side checks]

## State Synchronization

### Snapshot Contents
| Field | Type | Size | Rate | Compression |
|-------|------|------|------|-------------|
| [Field] | [Type] | [Bytes] | [Hz] | [Method] |

### Delta Compression
[How deltas are calculated and applied]

### Priority System
| Priority | Data Types | Behavior |
|----------|------------|----------|
| Critical | [Types] | Every packet |
| High | [Types] | Every other packet |
| Medium | [Types] | When bandwidth allows |
| Low | [Types] | Occasional |

## Edge Cases

| Scenario | Detection | Handling |
|----------|-----------|----------|
| High latency (>200ms) | [How detected] | [What happens] |
| Packet loss (>5%) | [How detected] | [What happens] |
| Jitter spike | [How detected] | [What happens] |
| Reconnection | [How detected] | [What happens] |

## Implementation Notes

### Key Classes/Functions
[Main components to implement]

### Dependencies
[Required libraries or systems]

### Testing Approach
[How to test with simulated network conditions]
```

Generate based on the user's game and networking requirements.
