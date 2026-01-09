---
name: dialogue-tree
description: Generate a branching dialogue structure for a conversation or scene
---

# Dialogue Tree Generator

Create a structured branching dialogue for a game conversation.

## Context Gathering

Before generating the dialogue tree, understand the context:

### Analyze the Scene
- Who are the characters involved?
- What's the setting and mood?
- What's the relationship between characters?
- What's the goal of this conversation?

### Understand Game Context
- Are there existing character voice guides?
- What dialogue format does the game use?
- Are there choice-consequence systems?
- What variables/flags are available?

### Check Narrative Requirements
- What information must be conveyed?
- What choices should players have?
- Are there skill checks or stat requirements?
- What outcomes are needed?

### Identify Constraints
- Maximum dialogue length?
- Voice acting considerations?
- Localization requirements?
- Branch complexity limits?

Use this context to create appropriate dialogue.

## Output Format

```markdown
# Dialogue Tree: [Scene Name]

## Overview
**Characters:** [Who's speaking]
**Location:** [Where this occurs]
**Trigger:** [What starts this dialogue]
**Purpose:** [What this accomplishes]

## Character Voices

### [Character Name]
**Tone:** [How they speak]
**Key traits:** [Verbal characteristics]
**Emotional state:** [In this scene]

[Repeat for each character]

## Dialogue Flow

### Entry
**Condition:** [What triggers this dialogue]
**Mood:** [Starting emotional tone]

---

**[CHARACTER]:** "[Opening line]"

[PLAYER CHOICE]
├─→ **"[Choice text 1]"**
│   └─ **[CHARACTER]:** "[Response to choice 1]"
│      └─ [Continue or branch...]
│
├─→ **"[Choice text 2]"**
│   └─ **[CHARACTER]:** "[Response to choice 2]"
│      └─ [Continue or branch...]
│
└─→ **"[Choice text 3]"** [if condition]
    └─ **[CHARACTER]:** "[Response to choice 3]"

---

### Branching Nodes

#### Node: [Branch Name]
**Reached via:** [How player gets here]

**[CHARACTER]:** "[Dialogue]"

[Continue structure...]

---

## Variables & Flags

| Variable | Set When | Value |
|----------|----------|-------|
| [var_name] | [Trigger] | [value] |

## End States

| Ending | Condition | Result |
|--------|-----------|--------|
| [Name] | [How reached] | [What happens next] |

## Implementation Notes
[Technical requirements, string IDs, etc.]
```

Generate based on the user's scene description and character details.
