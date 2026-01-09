---
name: playtest-plan
description: Create a structured playtesting session plan
---

# Playtest Plan Generator

Create a comprehensive playtesting session plan for gathering player feedback.

## Context Gathering

Before creating the playtest plan, understand the testing needs:

### Identify Testing Goals
- What specific questions need answers?
- What features or content are being tested?
- What success metrics matter?
- What hypotheses are being validated?

### Understand the Build
- What state is the build in?
- What's playable vs. placeholder?
- What known issues exist?
- What's the session length?

### Define Participants
- Who is the target player?
- How many participants needed?
- What screening criteria apply?
- What compensation is offered?

### Check Logistics
- Where will sessions happen?
- What equipment is available?
- Who will facilitate?
- What recording is possible?

Use this context to create an appropriate playtest plan.

## Output Format

```markdown
# Playtest Plan: [Session Name]

## Overview
**Build version:** [Version being tested]
**Date/time:** [Scheduled time]
**Duration:** [Session length per participant]
**Participants:** [Number and description]
**Location:** [Where sessions occur]

## Testing Objectives

### Primary Questions
1. [Critical question to answer]
2. [Critical question to answer]
3. [Critical question to answer]

### Secondary Questions
1. [Nice-to-know question]
2. [Nice-to-know question]

### Success Metrics
| Metric | Target | How Measured |
|--------|--------|--------------|
| [Metric] | [Target] | [Method] |

## Participant Profile

### Target Audience
**Demographics:** [Age, gaming background, etc.]
**Experience level:** [With genre/similar games]
**Platform familiarity:** [Controller/M+K/touch]

### Screening Questions
1. [Screening question to qualify participants]
2. [Screening question]
3. [Screening question]

### Recruitment
**Method:** [How participants are found]
**Target N:** [Number needed]
**Compensation:** [What participants receive]

## Session Structure

### Pre-Session (X minutes)
- Welcome and introductions
- Consent form and recording permission
- Brief context (without spoilers)
- Think-aloud instruction
- Equipment familiarization

### Play Session (X minutes)

#### Segment 1: [Name] (X min)
**Focus:** [What to observe]
**Starting point:** [Where they begin]
**Let them:** [What freedom they have]
**Watch for:** [Specific behaviors]

#### Segment 2: [Name] (X min)
**Focus:** [What to observe]
**Starting point:** [Where they begin]
**Let them:** [What freedom they have]
**Watch for:** [Specific behaviors]

[Additional segments as needed]

### Post-Session (X minutes)
- Structured debrief questions
- Open discussion
- Thank you and compensation

## Observation Guide

### Key Behaviors to Watch
- [ ] [Behavior 1 and what it indicates]
- [ ] [Behavior 2 and what it indicates]
- [ ] [Behavior 3 and what it indicates]

### Red Flags
- [Behavior that indicates serious problem]
- [Behavior that indicates serious problem]

### Success Indicators
- [Behavior that indicates feature working]
- [Behavior that indicates feature working]

## Debrief Questions

### Immediate Reactions
1. What's your overall impression?
2. What stood out to you most?
3. How did you feel while playing?

### Specific Probes
1. [Question about specific feature/area]
2. [Question about specific feature/area]
3. [Question about specific feature/area]

### Future Intent
1. Would you play this again? Why/why not?
2. Who do you think this game is for?
3. What would make you want to play more?

## Facilitator Notes

### Do's
- Observe without helping
- Ask "what are you thinking?" when they hesitate
- Note behaviors AND emotions
- Let them struggle (within reason)
- Remain neutral regardless of feedback

### Don'ts
- Don't explain solutions
- Don't lead with "did you find X confusing?"
- Don't defend design decisions
- Don't ask "do you like it?"
- Don't interrupt flow for questions

### Intervention Points
- Intervene if: [Specific blocking conditions]
- Do not intervene if: [Let them work through these]

## Data Collection

### During Session
| Time | Observation | Player Comment | Severity |
|------|-------------|----------------|----------|
| | | | |

### Quantitative Metrics
- Task 1 completion: [ ] Yes [ ] No — Time: ___
- Task 2 completion: [ ] Yes [ ] No — Time: ___
- [Additional task tracking]

### Recording
**Video:** [Yes/No - what's captured]
**Audio:** [Yes/No - what's captured]
**Screen:** [Yes/No - what's captured]
**Notes:** [Who takes notes]

## Logistics Checklist

### Before Sessions
- [ ] Build installed and verified stable
- [ ] Recording equipment tested
- [ ] Consent forms printed/ready
- [ ] Observation sheets prepared
- [ ] Compensation available
- [ ] Room/space set up
- [ ] Backup equipment ready

### Per Session
- [ ] Participant confirmed
- [ ] Fresh game state ready
- [ ] Recording started
- [ ] Consent obtained
- [ ] Notes template open

### After Sessions
- [ ] Files saved/backed up
- [ ] Quick observations noted
- [ ] Participant thanked/compensated
- [ ] Reset for next session

## Analysis Plan

### Immediate (Same Day)
- Facilitator debrief meeting
- Capture hot takes while fresh
- Flag critical issues

### Processing (Within Week)
- Transcribe key moments
- Code observations by theme
- Quantify completion rates
- Identify patterns across participants

### Reporting
- Summary document with findings
- Video clips of key moments
- Prioritized recommendations
- Share with team by [date]

## Schedule

| Slot | Time | Participant | Facilitator | Notes |
|------|------|-------------|-------------|-------|
| 1 | [Time] | [ID] | [Name] | |
| 2 | [Time] | [ID] | [Name] | |
| Buffer | [Time] | — | — | Catch-up if needed |
| 3 | [Time] | [ID] | [Name] | |

## Contingencies

**If participant no-shows:** [Backup plan]
**If build crashes:** [Recovery procedure]
**If running over time:** [What to cut]
**If participant gets stuck:** [Intervention threshold]
```

Generate a complete playtest plan based on the game and testing objectives.
