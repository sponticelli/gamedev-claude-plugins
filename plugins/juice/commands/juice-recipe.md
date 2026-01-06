---
name: juice-recipe
description: Get a specific juice recipe for a mechanic - detailed breakdown of exactly what feedback to add
---

# Juice Recipe

Get a complete, implementation-ready juice recipe for a specific game mechanic.

## Process

1. Identify the mechanic type
2. Determine intensity level (subtle/standard/bombastic)
3. Generate complete recipe across all pillars
4. Include timing specifications
5. Suggest implementation order

## Output Format

```markdown
## Juice Recipe: [Mechanic Name]

**Intensity Level:** [Subtle / Standard / Bombastic]
**Genre Context:** [What type of game this is for]

---

### Input Response

| Trigger | Effect | Timing |
|---------|--------|--------|
| [Button down] | [What happens] | [Instant/Xms delay] |
| [Button held] | [What happens] | [Duration behavior] |
| [Button release] | [What happens] | [Timing] |

**Sound:** [Sound description]
**Haptics:** [Vibration pattern if applicable]

---

### Visual Feedback

#### Screen Effects
| Effect | Parameters | Duration |
|--------|------------|----------|
| [Shake/Flash/Zoom] | [Intensity, direction] | [Xms] |

#### Particles
| Particle | Count | Behavior |
|----------|-------|----------|
| [Type] | [#-#] | [Burst/stream, physics, fade] |

#### Animation
| Element | Animation | Easing |
|---------|-----------|--------|
| [What moves] | [How it moves] | [Curve type] |

---

### Audio Feedback

| Layer | Sound | Variation |
|-------|-------|-----------|
| Primary | [Main sound] | [Pitch/timing variation] |
| Impact | [Hit sound] | [Based on intensity] |
| Sweetener | [Additional layer] | [When to include] |

**Mix Notes:** [Volume relationships, ducking, priorities]

---

### Animation Details

```
Timeline (60fps):
Frame 0:    [State/action]
Frame 1-3:  [Anticipation/build]
Frame 4-6:  [Peak action]
Frame 7-12: [Follow-through]
Frame 13+:  [Return to rest]
```

**Easing Curves:**
- [Element]: [Curve type and why]
- [Element]: [Curve type and why]

**Squash/Stretch:**
- Peak: [Scale values, e.g., 1.2x horizontal, 0.8x vertical]
- Rest: [Return values]

---

### Implementation Order

1. **First:** [Most impactful, lowest effort]
2. **Then:** [Next priority]
3. **After:** [Supporting elements]
4. **Finally:** [Polish touches]

---

### Variations

**Light version (weaker hit):**
[What to reduce/remove]

**Heavy version (stronger hit):**
[What to amplify/add]

**Combo/chain version:**
[What escalates with repeated actions]

---

### Reference
**Study this:** [Specific game + moment]
**Why:** [What to observe and learn]
```

## Mechanic Quick Reference

If user just says a mechanic name, use these defaults:

- **Jump:** Standard platformer feel
- **Attack:** Action game melee hit
- **Shoot:** Standard shooter fire
- **Collect:** Pickup/coin grab
- **Damage:** Player taking hit
- **Death:** Player death moment
- **Level Up:** RPG progression moment
- **Button Press:** UI interaction
