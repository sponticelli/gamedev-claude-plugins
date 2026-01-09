---
name: pwa-spec
description: Generate PWA specification for a web game
---

# PWA Specification Generator

Generate a comprehensive Progressive Web App specification for a browser game.

## Context Gathering

Before generating, understand:

### Game Context
- Game type and play patterns
- Offline capability requirements
- Data sync requirements
- Storage needs

### User Context
- Target platforms (desktop, mobile, both)
- Install prompt strategy
- Update behavior expectations

## Output Format

```markdown
# PWA Specification: [Game Name]

## Overview
**PWA Goal:** [What PWA features enable]
**Offline Support:** [Full/Partial/None]
**Install Priority:** [High/Medium/Low]

## Web App Manifest

```json
{
  "name": "[Full Game Name]",
  "short_name": "[Short Name - 12 chars max]",
  "description": "[Game description]",
  "start_url": "/?source=pwa",
  "display": "fullscreen",
  "orientation": "[landscape/portrait/any]",
  "background_color": "#[hex]",
  "theme_color": "#[hex]",
  "icons": [
    {
      "src": "/icons/icon-192.png",
      "sizes": "192x192",
      "type": "image/png",
      "purpose": "any maskable"
    },
    {
      "src": "/icons/icon-512.png",
      "sizes": "512x512",
      "type": "image/png"
    }
  ],
  "screenshots": [
    {
      "src": "/screenshots/gameplay.png",
      "sizes": "1280x720",
      "type": "image/png",
      "form_factor": "wide"
    }
  ],
  "categories": ["games"],
  "prefer_related_applications": false
}
```

## Service Worker Strategy

### Caching Tiers
| Tier | Assets | Strategy | Max Age |
|------|--------|----------|---------|
| Shell | HTML, core JS/CSS | Cache first | Versioned |
| Game assets | Sprites, audio | Stale-while-revalidate | 7 days |
| API responses | Leaderboards, saves | Network first | 1 hour |
| Dynamic | User content | Network only | N/A |

### Precache List
```javascript
const PRECACHE = [
  '/',
  '/index.html',
  '/main.js',
  '/style.css',
  '/manifest.json',
  // Core game assets
  '/assets/player.png',
  '/assets/ui.png',
  '/audio/bgm.mp3'
];
```

### Runtime Caching Rules
```javascript
// Game assets: stale-while-revalidate
workbox.routing.registerRoute(
  /\/assets\//,
  new workbox.strategies.StaleWhileRevalidate({
    cacheName: 'game-assets',
    plugins: [
      new workbox.expiration.ExpirationPlugin({
        maxEntries: 100,
        maxAgeSeconds: 7 * 24 * 60 * 60
      })
    ]
  })
);

// API: network first with cache fallback
workbox.routing.registerRoute(
  /\/api\//,
  new workbox.strategies.NetworkFirst({
    cacheName: 'api-cache',
    networkTimeoutSeconds: 5
  })
);
```

## Offline Capabilities

### Fully Offline
- [x] Core gameplay
- [x] Local save games
- [ ] (Optional) Previously loaded levels

### Requires Network
- [ ] Leaderboards (show cached)
- [ ] Purchases
- [ ] Multiplayer

### Sync Strategy
| Data Type | Offline Behavior | Sync Trigger |
|-----------|------------------|--------------|
| Save games | Queue for sync | On reconnect |
| High scores | Store locally | Background sync |
| Purchases | Not available | N/A |

## Storage Plan

### Quotas
| Storage Type | Purpose | Estimated Size |
|--------------|---------|----------------|
| Cache API | Game shell & assets | [X] MB |
| IndexedDB | Save data, sync queue | [X] MB |
| LocalStorage | Settings, preferences | [X] KB |

### Persistence
```javascript
// Request persistent storage
if (navigator.storage && navigator.storage.persist) {
  const isPersisted = await navigator.storage.persist();
  // Handle based on result
}
```

## Install Experience

### Prompt Timing
**Show when:** [After N minutes of play / After completing tutorial / On return visit]
**Don't show if:** [Already installed, previously declined within 7 days]

### Custom Install UI
- [Description of custom UI approach]
- [Deferred prompt handling]

### Post-Install
- [Any special post-install behavior]
- [How experience changes when installed]

## Update Strategy

### Service Worker Updates
**Check frequency:** On each visit
**Notification:** [Silent / Prompt / Force after X days]

### Update Flow
1. New SW detected
2. [Behavior during update]
3. [Activation strategy]

## Push Notifications (if applicable)

### Use Cases
- [ ] Daily challenge reminder
- [ ] Friend activity
- [ ] Event announcements

### Permission Request
**When:** [After explicit user interest]
**Fallback:** [In-game notification system]

## Testing Checklist

### Installation
- [ ] Install prompt appears appropriately
- [ ] App installs correctly
- [ ] Icons display properly
- [ ] Launch from home screen works

### Offline
- [ ] Game loads offline
- [ ] Gameplay works offline
- [ ] Saves persist offline
- [ ] UI indicates offline state

### Updates
- [ ] SW updates detected
- [ ] Update flow is smooth
- [ ] No data loss on update
```

Generate the PWA specification based on the game context provided.
