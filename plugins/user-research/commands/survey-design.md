---
name: survey-design
description: Design a player survey with effective question design
---

# Survey Design Generator

Create a well-designed player survey for gathering quantitative and qualitative feedback.

## Context Gathering

Before designing the survey, understand the research goals:

### Define Research Questions
- What decisions will this data inform?
- What hypotheses are being tested?
- What's the priority question?
- What secondary insights are valuable?

### Identify Target Respondents
- Who should take this survey?
- How will they be recruited?
- What's the expected response rate?
- What sample size is needed?

### Understand Constraints
- How long can the survey be?
- What platform will it use?
- Is there incentive/compensation?
- When are results needed?

### Check Existing Data
- What do we already know?
- What questions remain unanswered?
- What telemetry can supplement?
- Are there baseline metrics to compare?

Use this context to design an effective survey.

## Output Format

```markdown
# Survey Design: [Survey Name]

## Overview
**Purpose:** [What this survey measures]
**Target audience:** [Who takes it]
**Estimated time:** [X minutes]
**Distribution:** [How it reaches players]
**Incentive:** [Compensation if any]

## Research Questions

### Primary
1. [Key question this survey must answer]
2. [Key question this survey must answer]

### Secondary
1. [Additional insight to gather]
2. [Additional insight to gather]

## Survey Structure

### Section 1: Screening (if needed)
**Purpose:** Ensure respondent qualifies

---

**Q1. [Screening question]**
- Option A
- Option B
- Option C

*Logic: If [condition], continue. Otherwise, thank and exit.*

---

### Section 2: Experience Context
**Purpose:** Understand respondent's background with the game

---

**Q2. How long have you been playing [Game]?**
- Less than a week
- 1-4 weeks
- 1-3 months
- 3-6 months
- More than 6 months

---

**Q3. How often do you typically play [Game]?**
- Daily
- A few times a week
- About once a week
- A few times a month
- Less than once a month

---

**Q4. Which platform do you primarily play on?**
- PC
- PlayStation
- Xbox
- Nintendo Switch
- Mobile
- Other: ______

---

### Section 3: Core Questions
**Purpose:** Gather primary research data

---

**Q5. [Rating question about key topic]**
*Please rate your agreement with the following statement:*

"[Statement to evaluate]"

| Strongly Disagree | Disagree | Neutral | Agree | Strongly Agree |
|:-:|:-:|:-:|:-:|:-:|
| 1 | 2 | 3 | 4 | 5 |

---

**Q6. [Feature satisfaction question]**
*How satisfied are you with [feature/aspect]?*

| Very Dissatisfied | Dissatisfied | Neutral | Satisfied | Very Satisfied |
|:-:|:-:|:-:|:-:|:-:|
| 1 | 2 | 3 | 4 | 5 |

---

**Q7. [Frequency/behavior question]**
*How often do you [behavior]?*
- Never
- Rarely
- Sometimes
- Often
- Always

---

**Q8. [Multiple choice - single answer]**
*Which of the following best describes [topic]?*
- Option A
- Option B
- Option C
- Option D
- Other: ______

---

**Q9. [Multiple choice - multiple answers]**
*Which of the following [topics] have you experienced? (Select all that apply)*
- [ ] Option A
- [ ] Option B
- [ ] Option C
- [ ] Option D
- [ ] None of the above

---

**Q10. [Ranking question]**
*Please rank the following [items] from most to least [criterion] (1 = most, 4 = least):*
- __ Item A
- __ Item B
- __ Item C
- __ Item D

---

### Section 4: Open-Ended Feedback
**Purpose:** Capture qualitative insights

---

**Q11. [Open-ended about positive experience]**
*What do you enjoy most about [Game/feature]?*

[Text field - 500 character limit]

---

**Q12. [Open-ended about improvement]**
*If you could change one thing about [Game/feature], what would it be?*

[Text field - 500 character limit]

---

**Q13. [Open-ended for unexpected insights]**
*Is there anything else you'd like to share about your experience?*

[Text field - 1000 character limit]
*Optional*

---

### Section 5: Demographics (if needed)
**Purpose:** Enable segment analysis

---

**Q14. What is your age range?**
- Under 18
- 18-24
- 25-34
- 35-44
- 45-54
- 55+
- Prefer not to say

---

**Q15. How would you describe your gaming experience level?**
- Casual - I play games occasionally for fun
- Regular - I play games several times a week
- Dedicated - Gaming is one of my main hobbies
- Hardcore - I invest significant time mastering games

---

### Closing
**Thank you for your feedback!**

[Optional: Information about incentive redemption]
[Optional: Link to community/updates]

---

## Question Design Notes

### Why These Questions Work
| Question | Design Choice | Rationale |
|----------|---------------|-----------|
| Q2 | Time ranges, not exact | Easier to answer accurately |
| Q5-6 | 5-point Likert | Standard, allows neutral |
| Q11-12 | Separate positive/negative | Prevents bias toward criticism |
| Q13 | Optional | Reduces abandonment |

### Questions Avoided
- ~~"Do you like X?"~~ → Too vague, use satisfaction scale
- ~~"Don't you agree that..."~~ → Leading
- ~~"How satisfied with graphics and gameplay?"~~ → Double-barreled
- ~~"Rate 1-100"~~ → Too granular for reliable data

## Skip Logic

| Condition | Action |
|-----------|--------|
| Q1 = [disqualifying answer] | Thank and exit |
| Q3 = "Less than once a month" | Skip to Q[X] |
| [Other conditions] | [Other actions] |

## Analysis Plan

### Quantitative Analysis
| Question | Analysis Method | Output |
|----------|-----------------|--------|
| Q2-4 | Frequency distribution | Respondent profile |
| Q5-6 | Mean, distribution | Satisfaction metrics |
| Q7 | Cross-tab with Q5 | Behavior-satisfaction correlation |
| Q9 | Frequency counts | Feature exposure rates |

### Qualitative Analysis
| Question | Coding Approach | Expected Themes |
|----------|-----------------|-----------------|
| Q11 | Positive sentiment themes | [Theme 1], [Theme 2] |
| Q12 | Pain point categories | [Category 1], [Category 2] |
| Q13 | Open coding | Emergent themes |

### Segment Comparisons
- Compare Q5-6 by Q2 (tenure groups)
- Compare Q5-6 by Q15 (player type)
- Compare Q12 themes by Q3 (engagement level)

## Sample Size Requirements

**Target N:** [Number]
**Rationale:** [Why this number]
**Margin of error:** ±[X]% at 95% confidence (for proportions)

### Segment Minimums
| Segment | Minimum N | Priority |
|---------|-----------|----------|
| [Segment 1] | [N] | High |
| [Segment 2] | [N] | Medium |

## Distribution Plan

### Channel
**Primary:** [In-game prompt / Email / Discord / etc.]
**Timing:** [When survey appears]
**Duration:** [How long survey is open]

### Invitation Text
> [Draft invitation message that explains purpose, time commitment, and incentive]

### Reminders
- Reminder 1: [Timing and channel]
- Reminder 2: [Timing and channel]

## Quality Checks

### Before Launch
- [ ] All questions are clear and unambiguous
- [ ] No leading or biased wording
- [ ] Response options are mutually exclusive and exhaustive
- [ ] Skip logic tested
- [ ] Mobile-friendly formatting verified
- [ ] Estimated time is accurate
- [ ] Pilot tested with 5+ people

### During Collection
- [ ] Monitor completion rate (target: >70%)
- [ ] Check for straight-lining patterns
- [ ] Review open-ended responses for confusion

### Data Cleaning
- Remove responses under [X] minutes (speeders)
- Remove responses with [pattern] (bots/low effort)
- Flag incomplete responses for separate analysis
```

Generate a complete survey design based on the research objectives.
