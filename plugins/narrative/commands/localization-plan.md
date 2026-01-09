---
name: localization-plan
description: Generate a localization strategy and execution plan
---

# Localization Plan Generator

Create a comprehensive localization strategy document.

## Context Gathering

Before generating the localization plan, understand the project:

### Analyze Target Markets
- What regions/languages are priorities?
- What's the expected player distribution?
- Are there platform-specific requirements?
- What are the key markets for revenue?

### Understand Content Scope
- How much text content exists?
- Is voice acting included?
- What's the content update frequency?
- Are there culturally sensitive elements?

### Check Technical Setup
- What string management system exists?
- How are strings extracted?
- What format are strings stored in?
- What's the localization tool pipeline?

### Identify Constraints
- Budget for localization?
- Timeline requirements?
- Team capacity?
- Quality vs. speed priorities?

Use this context to create a realistic localization plan.

## Output Format

```markdown
# Localization Plan: [Game Name]

## Executive Summary
**Target Languages:** [Number and list]
**Localization Level:** [Text only / Full / Culturalized]
**Estimated Timeline:** [Duration]
**Budget Range:** [Estimate]

## Market Priority

### Tier 1: Launch Languages
| Language | Market Size | Priority Reason |
|----------|-------------|-----------------|
| [Language] | [Size/importance] | [Why prioritized] |

### Tier 2: Fast Follow
| Language | Target Date | Notes |
|----------|-------------|-------|
| [Language] | [When] | [Considerations] |

### Tier 3: Future Consideration
[Languages to evaluate based on success]

## Content Audit

### Text Content
| Content Type | Word Count | Complexity |
|--------------|------------|------------|
| UI | [Count] | [Low/Med/High] |
| Dialogue | [Count] | [Low/Med/High] |
| Items/Descriptions | [Count] | [Low/Med/High] |
| Tutorials | [Count] | [Low/Med/High] |
| Marketing | [Count] | [Low/Med/High] |
| **Total** | **[Total]** | - |

### Voice Content (if applicable)
| Content | Duration | Languages |
|---------|----------|-----------|
| [Type] | [Hours] | [Which langs] |

### Special Considerations
[Cultural adaptations, sensitive content, etc.]

## Technical Requirements

### String Management
**Tool:** [Platform/system]
**Format:** [File format]
**ID Convention:** [Pattern]

### Integration
[How localization integrates with builds]

### Font Support
| Language | Font Requirements |
|----------|-------------------|
| [Lang] | [Font/rendering needs] |

### UI Accommodations
- Text expansion: [Approach]
- RTL support: [If needed]
- Dynamic text: [How handled]

## Workflow

### Phase 1: Setup
- [ ] Configure localization tool
- [ ] Extract all strings
- [ ] Provide context/screenshots
- [ ] Create glossary

### Phase 2: Translation
- [ ] Tier 1 languages
- [ ] Review cycle
- [ ] Integration

### Phase 3: LQA
- [ ] Functional testing
- [ ] Linguistic review
- [ ] Cultural review
- [ ] Bug fixing

### Phase 4: Launch
- [ ] Final review
- [ ] Build integration
- [ ] Store listing translation
- [ ] Marketing materials

## Timeline

| Milestone | Date | Languages |
|-----------|------|-----------|
| Strings final | [Date] | All |
| Translation complete | [Date] | Tier 1 |
| LQA complete | [Date] | Tier 1 |
| Launch | [Date] | Tier 1 |
| Tier 2 complete | [Date] | Tier 2 |

## Budget Breakdown

| Component | Tier 1 | Tier 2 | Total |
|-----------|--------|--------|-------|
| Translation | $[X] | $[Y] | $[Z] |
| Voice (if any) | $[X] | $[Y] | $[Z] |
| LQA | $[X] | $[Y] | $[Z] |
| Tools | $[X] | - | $[X] |
| **Total** | **$[X]** | **$[Y]** | **$[Z]** |

## Quality Assurance

### LQA Process
[Testing approach for each phase]

### Acceptance Criteria
[What defines "done" for each language]

### Issue Tracking
[How localization bugs are tracked and fixed]

## Ongoing Maintenance

### Content Updates
[How new content is localized]

### Community Feedback
[How player feedback is handled]

### Translation Memory
[How past translations are reused]

## Risks & Mitigations

| Risk | Likelihood | Impact | Mitigation |
|------|------------|--------|------------|
| [Risk] | [H/M/L] | [H/M/L] | [Strategy] |
```

Generate based on the user's game and localization requirements.
