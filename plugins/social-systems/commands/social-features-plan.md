---
name: social-features-plan
description: Design in-game social features and player connection systems
---

# Social Features Plan Generator

Create a comprehensive plan for in-game social features and player connections.

## Context Gathering

Before designing social features, understand the context:

### Understand the Game
- What type of game is this?
- Is it competitive, cooperative, or both?
- What's the session structure?
- What's the target audience?

### Define Social Goals
- Why should players connect?
- What social behaviors to encourage?
- What social behaviors to prevent?
- How important is retention through social?

### Check Platform Requirements
- What platforms are targeted?
- What platform social features exist?
- What are the age rating implications?
- What privacy regulations apply?

### Identify Resources
- What moderation capacity exists?
- What's the development budget?
- What maintenance is sustainable?
- What analytics are available?

Use this context to design appropriate social features.

## Output Format

```markdown
# Social Features Plan: [Game Name]

## Overview

### Social Vision
**Core philosophy:** [One sentence describing social approach]
**Key value:** [Primary benefit players get from social features]
**Tone:** [Competitive/Friendly/Community-focused/etc.]

### Success Metrics
| Metric | Definition | Target |
|--------|------------|--------|
| Friend connections | [How measured] | [Target] |
| Social sessions | % sessions with friends | [Target] |
| Social retention | D7 for players with friends vs without | [Lift target] |
| Report rate | Reports per 1000 sessions | [Max acceptable] |

---

## Friend System

### Friend Discovery

#### Adding Friends
| Method | Implementation | Priority |
|--------|----------------|----------|
| Post-match suggestion | "Add recent teammates" prompt | High |
| Username search | Search by exact username | High |
| QR code/link | Generate shareable friend link | Medium |
| Platform import | Connect Steam/PSN/etc. friends | Medium |
| Recommendations | "Suggested friends" algorithm | Low |

#### Friend Requests
**Request flow:**
1. Player A sends request
2. Player B sees notification
3. Player B accepts/declines/ignores
4. If accepted, mutual friend status

**Spam prevention:**
- Max pending requests: [#]
- Cooldown after decline: [Time]
- Block prevents future requests

### Friend Management

#### Friend List
**Display information:**
- Username and avatar
- Online status (with privacy options)
- Current activity (if sharing)
- Favorite star indicator
- Last played together

**Organization:**
- Favorites (pinned to top)
- Recent (recently played with)
- Online (currently available)
- Offline (sorted by recency)

**Limits:**
- Maximum friends: [#]
- Maximum favorites: [#]

#### Friend Actions
| Action | Description | Access |
|--------|-------------|--------|
| Message | Send direct message | Always |
| Invite | Invite to current session | When possible |
| Join | Join their session | If allowed |
| Spectate | Watch their game | If allowed |
| View profile | See their stats/achievements | Always |
| Unfriend | Remove friendship | Always |
| Block | Block all contact | Always |

### Presence System

#### Status Options
| Status | Meaning | Shown as |
|--------|---------|----------|
| Online | Playing, available | Green dot |
| In-game | In match, limited availability | Yellow dot |
| Away | Idle | Gray dot |
| Do Not Disturb | No notifications | Red dot |
| Invisible | Appear offline to friends | (hidden) |
| Offline | Not connected | No dot |

#### Activity Sharing
**Shared by default:**
- Online/offline status
- General activity (main menu, in match)

**Opt-in sharing:**
- Specific game mode
- Match progress
- Joinability

**Privacy settings:**
- Share with: All friends / Close friends / Nobody
- Per-friend overrides: [Yes/No]

---

## Communication

### Text Chat

#### Direct Messages
**Features:**
- 1:1 conversations
- Message history: [Duration retained]
- Read receipts: [Yes/No]
- Typing indicator: [Yes/No]

**Moderation:**
- Profanity filter: [Type]
- Link filtering: [Rules]
- Image sharing: [Allowed/Not allowed]
- Report button on each message

#### Group Chat
**Creation:**
- Max participants: [#]
- Who can create: [Everyone/Friends only]
- Who can invite: [Creator/Anyone in group]

**Features:**
- Naming groups
- Leaving groups
- Muting notifications

#### In-Game Chat
| Context | Scope | Type | Moderation |
|---------|-------|------|------------|
| Match | Team | Text | Filtered |
| Match | All | Text | Filtered |
| Lobby | Party | Text | Filtered |
| Public | Region/global | Text | Heavy filter + delay |

### Quick Communication

#### Emote/Ping System
**Purpose:** Enable communication without text

**Types:**
| Category | Examples | Uses |
|----------|----------|------|
| Tactical | "Attack here", "Defend", "Retreat" | Gameplay coordination |
| Social | Wave, Thumbs up, Clap | Positive interaction |
| Emotional | Happy, Sad, Confused | Expression |
| Functional | "Yes", "No", "Help" | Quick responses |

**Accessibility notes:**
- Clear visual indicators
- Audio cues (optional)
- Not just color-coded

#### Compliment System
**Post-match compliments:**
- Good teammate
- Fun opponent
- Great play
- [Game-specific compliments]

**Benefits:**
- Sender: [Reward if any]
- Receiver: [Display, stats, rewards]

### Voice Chat

#### Availability
| Mode | Voice Support | Default State |
|------|---------------|---------------|
| Matchmade | Team voice | Off, opt-in |
| Party | Party voice | On |
| Spectating | [Yes/No] | [State] |

#### Controls
**User controls:**
- Mute self (global toggle)
- Mute others (per-player)
- Voice volume slider
- Push-to-talk option
- Voice activation threshold

**Moderation:**
- Report for voice abuse
- Temporary voice ban
- Permanent voice ban

---

## Social Activities

### Playing Together

#### Party System
**Features:**
- Invite to party
- Party leader controls
- Ready check
- Party chat
- Cross-platform (if applicable)

**Limits:**
- Max party size: [#]
- Matchmaking together: [Rules]

#### Invite System
| Method | Description | Deep link |
|--------|-------------|-----------|
| In-game | Send from friends list | N/A |
| Share link | Generate URL | Yes |
| Platform | Use Steam/PSN/etc. | Platform-specific |

#### Join-in-Progress
**Joinability:**
- Who can join: [Friends/Party/Invite only/Nobody]
- When joins are allowed: [Pre-match/Anytime/Never mid-match]
- Backfill behavior: [How late-joiners are handled]

### Sharing Features

#### Shareable Content
| Content | Platform | Discovery |
|---------|----------|-----------|
| Screenshots | In-game, External | Profile, Feed |
| Clips | In-game, External | Profile, Feed |
| Achievements | Automatic | Profile, Feed |
| Stats | Opt-in | Profile |
| Loadouts/builds | In-game | Community |

#### Activity Feed
**Content sources:**
- Friend achievements
- Friend milestones
- Community highlights
- Developer announcements

**Controls:**
- Filter by content type
- Hide specific friends
- Adjust frequency

### Competition

#### Leaderboards
| Type | Scope | Reset | Visibility |
|------|-------|-------|------------|
| Global | All players | [Season/Never] | Public |
| Friends | My friends | [Season/Never] | Friends |
| Regional | [Region] | [Season/Never] | Public |

#### Challenges
**Friend challenges:**
- Challenge friend to beat score
- Asynchronous (no need to be online together)
- Time-limited
- Optional wager (cosmetics, bragging rights)

---

## Safety & Moderation

### Player Protection

#### Blocking
**What blocking does:**
- Cannot send messages
- Cannot invite/join
- Cannot see in matchmaking (if feasible)
- Cannot view profile (optional)

**Block list:**
- Maximum blocks: [# or unlimited]
- Block list management UI
- Mutual: [If I block you, do you know?]

#### Reporting
**Report flow:**
1. Select player
2. Choose category
3. Add details (optional)
4. Submit
5. Confirmation shown

**Report categories:**
- Harassment/abuse
- Hate speech
- Cheating
- Inappropriate content
- Spam
- Other

**Follow-up:**
- Acknowledge receipt: [Immediately]
- Outcome notification: [Yes/No]

### Content Moderation

#### Text Filtering
**Approach:** [Real-time filter / Post-hoc review / Both]

**Filter types:**
- Profanity: [Block/Replace/Allow]
- Slurs: [Block/Replace]
- Personal info: [Warn/Block]
- Links: [Whitelist/Block/Allow]

#### Behavior Monitoring
**Tracked behaviors:**
- Report frequency (sender and recipient)
- Mute frequency
- Block frequency
- Chat volume

**Automated actions:**
- [Threshold] → Warning
- [Threshold] → Temporary restriction
- [Threshold] → Permanent ban

### Privacy

#### Default Settings
| Setting | Default | Changeable |
|---------|---------|------------|
| Friend requests | From anyone | Yes |
| Messages | Friends only | Yes |
| Activity visibility | Friends | Yes |
| Profile visibility | Public | Yes |
| Join permissions | Friends | Yes |

#### Age-Appropriate Design
**For minors (<18):**
- Chat restricted to friends by default
- No public profile
- Parental controls available

**For children (<13, if applicable):**
- [COPPA compliance measures]
- [Additional restrictions]

---

## Technical Requirements

### Data Storage
| Data Type | Retention | GDPR Consideration |
|-----------|-----------|-------------------|
| Friend list | Permanent | Exportable/Deletable |
| Messages | [Duration] | Exportable/Deletable |
| Reports | [Duration] | Internal only |
| Blocks | Permanent | Deletable |

### Cross-Platform
**Unified account:**
- Friends list shared across platforms
- Messages synced
- Settings synced

**Platform-specific:**
- Voice uses platform services
- Reporting integrates with platform
- Achievements platform-specific

### Performance
| Feature | Latency Target | Availability Target |
|---------|----------------|---------------------|
| Presence | <5s update | 99.9% |
| Messages | <1s delivery | 99.9% |
| Matchmaking | <30s | 99.5% |

---

## Launch Plan

### Phase 1: Core Social
- Friend system (add, remove, block)
- Direct messaging
- Party system
- Basic presence

### Phase 2: Communication
- Group chat
- In-game chat
- Quick communication
- Voice chat

### Phase 3: Engagement
- Activity feed
- Leaderboards
- Challenges
- Sharing features

### Phase 4: Refinement
- Recommendation system
- Advanced moderation
- Analytics-driven improvements
```

Generate a comprehensive social features plan based on the game and objectives.
