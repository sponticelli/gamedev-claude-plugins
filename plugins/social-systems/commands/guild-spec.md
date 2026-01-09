---
name: guild-spec
description: Create a guild/clan system specification
---

# Guild Specification Generator

Create a comprehensive guild/clan system specification for your game.

## Context Gathering

Before creating the guild specification, understand the requirements:

### Understand Game Context
- What type of game is this?
- What's the player progression system?
- Is the game PvE, PvP, or mixed?
- What's the target audience?

### Define Guild Purpose
- Why do players need guilds?
- What will guilds do together?
- How competitive should guilds be?
- What social role do guilds serve?

### Check Technical Constraints
- What's the server architecture?
- What's the max concurrent users?
- What platform(s)?
- What's the persistence model?

### Identify Monetization
- Will guilds have premium features?
- Can guilds purchase advantages?
- What's the fairness philosophy?
- How does this affect design?

Use this context to create an appropriate specification.

## Output Format

```markdown
# Guild System Specification: [Game Name]

## Overview

### Purpose
**Why guilds exist in this game:**
[Core value proposition for guild system]

**Player motivations served:**
- [Motivation 1]
- [Motivation 2]
- [Motivation 3]

### Key Metrics
| Metric | Target | Measurement |
|--------|--------|-------------|
| % players in guilds | [%] | [How measured] |
| Average guild size | [#] | [How measured] |
| Guild retention | [%] | [How measured] |

---

## Guild Structure

### Size Limits
**Minimum:** [# members to create]
**Starting maximum:** [# members at level 1]
**Maximum:** [Absolute cap at max level]
**Rationale:** [Why these numbers]

### Creation Requirements
| Requirement | Value | Rationale |
|-------------|-------|-----------|
| Founder level | [Level] | [Why] |
| Creation cost | [Currency/amount] | [Why] |
| Required founders | [#] | [Why] |
| Cooldown | [Time] | [Why] |

### Identity System
**Name:**
- Length: [Min-max characters]
- Allowed characters: [A-Z, etc.]
- Uniqueness: [Server/global]
- Change policy: [Cost, cooldown]

**Tag:**
- Length: [# characters]
- Display: [Where shown]
- Change policy: [Rules]

**Emblem/Crest:**
- Customization options: [Layers, colors, etc.]
- Unlock requirements: [How to get options]
- Display locations: [Where visible]

---

## Hierarchy & Permissions

### Roles

#### Guild Leader
**Slots:** 1
**Permissions:**
- Full administrative control
- Transfer leadership
- Disband guild
- All lower permissions

**Succession rules:**
- Inactivity threshold: [Days]
- Auto-transfer to: [Next highest rank]
- Manual transfer: [Requirements]

#### Officers
**Slots:** [Maximum #]
**Permissions:**
- Invite members
- Kick members (below rank)
- Access guild bank (tier X)
- Start guild events
- Manage announcements

#### [Additional Ranks]
[Define each rank with slots and permissions]

### Permission Matrix
| Permission | Leader | Officer | Senior | Member | Recruit |
|------------|--------|---------|--------|--------|---------|
| Invite members | ✓ | ✓ | ✓ | | |
| Kick members | ✓ | ✓ | | | |
| Bank deposit | ✓ | ✓ | ✓ | ✓ | |
| Bank withdraw | ✓ | Tier 2 | Tier 1 | | |
| Start events | ✓ | ✓ | | | |
| Announcements | ✓ | ✓ | | | |
| Edit settings | ✓ | | | | |
| Promote | ✓ | ✓ | | | |
| Demote | ✓ | ✓ | | | |

---

## Progression System

### Guild Leveling

**XP Sources:**
| Activity | XP Amount | Daily Cap | Notes |
|----------|-----------|-----------|-------|
| Member login | [XP] | [Cap] | Per member |
| [Content] completion | [XP] | [Cap] | Guild completion |
| Guild quest | [XP] | [Cap] | Weekly quests |
| Donations | [XP] | [Cap] | Currency conversion |
| [Other activity] | [XP] | [Cap] | [Notes] |

**Level Requirements:**
| Level | XP Required | Total XP | Unlock |
|-------|-------------|----------|--------|
| 1 | 0 | 0 | Base guild |
| 2 | [XP] | [Total] | [Feature] |
| 3 | [XP] | [Total] | [Feature] |
| ... | ... | ... | ... |
| Max | [XP] | [Total] | [Feature] |

### Unlockable Features
| Level | Feature | Description |
|-------|---------|-------------|
| 1 | Basic chat | Guild-wide text chat |
| 5 | Guild bank | Shared storage unlocked |
| 10 | +10 members | Member cap increase |
| 15 | Guild quests | Weekly objectives |
| 20 | Guild buffs | Passive bonuses |
| ... | ... | ... |

---

## Economic System

### Guild Bank

**Storage Slots:**
| Level | Currency Slots | Item Slots | Special Slots |
|-------|---------------|------------|---------------|
| 5 | [#] | [#] | [#] |
| 10 | [#] | [#] | [#] |
| ... | ... | ... | ... |

**Deposit Rules:**
- All members can deposit: [Items/Currency]
- Deposit limits: [Per day/total]
- Automatic deposits: [Tax on earnings]

**Withdrawal Rules:**
- Permission level required: [By item tier]
- Daily limits: [By rank]
- Approval required: [For valuable items]
- Audit logging: [What's tracked]

### Guild Funds

**Income:**
| Source | Amount | Frequency |
|--------|--------|-----------|
| Activity tax | [%] of member earnings | Automatic |
| Territory income | [Amount] | Per [time] |
| Event rewards | [Amount] | Per event |
| Donations | Variable | Player choice |

**Expenses:**
| Expense | Cost | Frequency |
|---------|------|-----------|
| Territory upkeep | [Amount] | Per [time] |
| Buff maintenance | [Amount] | Per buff/time |
| Event hosting | [Amount] | Per event |
| Upgrades | [Amount] | One-time |

---

## Activities

### Guild Quests
**Frequency:** [Daily/Weekly]
**Difficulty tiers:** [Number of tiers]
**Reward types:** [XP, currency, items]

**Quest Examples:**
| Quest | Target | Reward |
|-------|--------|--------|
| Collective defeats | Kill X enemies (guild total) | [Reward] |
| Guild dungeons | Complete X dungeons | [Reward] |
| Resource gathering | Gather X materials | [Reward] |

### Guild Events
[Major guild activities, raids, wars, etc.]

### Cooperative Content
[Content designed specifically for guild groups]

---

## Social Features

### Communication
**Guild chat:** [Features]
**Officer chat:** [Features]
**Announcements:** [MOTD, scheduled]
**Calendar:** [Event scheduling]

### Member Management
**Recruitment mode:**
- Open (anyone joins)
- Application (review required)
- Invite-only (must be invited)

**Tracking:**
- Last online: [Visibility]
- Activity score: [Calculation]
- Contribution: [What's tracked]

**Moderation:**
- Warning system: [Yes/No]
- Temporary ban: [Yes/No]
- Kick with reason: [Required/Optional]
- Blacklist: [Guild-level/shared]

---

## Technical Specification

### Data Model
```
Guild {
  id: unique_id
  name: string
  tag: string
  level: integer
  xp: integer
  created_at: timestamp
  leader_id: player_id
  settings: GuildSettings
  bank: GuildBank
  members: [GuildMember]
}

GuildMember {
  player_id: player_id
  rank: enum
  joined_at: timestamp
  contribution: integer
  last_active: timestamp
}
```

### API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| /guilds | POST | Create guild |
| /guilds/{id} | GET | Get guild info |
| /guilds/{id}/members | GET | List members |
| /guilds/{id}/invite | POST | Invite player |
| /guilds/{id}/leave | POST | Leave guild |
| ... | ... | ... |

### Scalability
**Expected guilds:** [# at launch, # at scale]
**Expected largest guild:** [# members]
**Sharding strategy:** [If applicable]

---

## Edge Cases

### Inactive Guilds
**Inactivity threshold:** [Days with no activity]
**Warning period:** [Days before action]
**Action taken:** [Dissolution/Freeze/Transfer]

### Leadership Absence
**Threshold:** [Days without leader login]
**Succession:** [Auto-transfer rules]
**Member notification:** [How informed]

### Guild Disputes
**Handling:** [Support intervention rules]
**What can be restored:** [Items, ranks, etc.]
**What cannot be undone:** [Disbanding, etc.]

---

## Monetization (if applicable)

### Premium Guild Features
| Feature | Price | Effect |
|---------|-------|--------|
| [Feature] | [Price] | [Description] |

### Fairness Guardrails
[How to prevent pay-to-win]
```

Generate a complete guild specification based on the game and requirements.
