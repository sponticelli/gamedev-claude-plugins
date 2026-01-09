---
name: rpc-design
description: Design an RPC/messaging system with serialization strategy for multiplayer games
---

# RPC/Messaging Design Generator

Create an RPC and messaging system design for multiplayer game communication.

## Context Gathering

Before generating the RPC design, understand the communication needs:

### Analyze Communication Patterns
- What player actions need server validation? (attacks, purchases, etc.)
- What events need to be broadcast to all players?
- What's private to individual players?
- Is there player-to-player messaging? (chat, trading)

### Understand Performance Requirements
- What's the expected message rate?
- What latency is acceptable for different message types?
- What's the bandwidth budget?
- Are there mobile data constraints?

### Check Technical Stack
- What language/framework is the server?
- What networking layer is used? (WebSocket, raw UDP, etc.)
- Are there existing RPC patterns to follow?
- Any serialization library preferences?

### Identify Security Needs
- What actions need rate limiting?
- What validation is required on each RPC?
- How are players authenticated?
- Is message encryption required?

Use this context to design appropriate RPC and messaging patterns.

## Output Format

```markdown
# RPC/Messaging Design: [Game/Feature]

## Overview
**Transport:** [WebSocket / TCP / UDP / gRPC]
**Serialization:** [JSON / MessagePack / Protobuf]
**Auth Model:** [JWT / Session / API Key]

## Message Envelope

### Standard Envelope
```json
{
  "type": "[rpc|event|request|response]",
  "id": "unique_message_id",
  "timestamp": 1234567890,
  "payload": { ... }
}
```

### Error Response
```json
{
  "type": "error",
  "id": "original_request_id",
  "error": {
    "code": "ERROR_CODE",
    "message": "Human readable message",
    "details": { ... }
  }
}
```

## RPCs (Client -> Server)

| Method | Parameters | Returns | Auth | Rate Limit |
|--------|------------|---------|------|------------|
| [method] | [params] | [return] | [Yes/No] | [X/sec] |

### RPC Definitions

#### [method_name]
**Purpose:** [What this RPC does]
**Request:**
```json
{
  "param1": "type",
  "param2": "type"
}
```
**Response:**
```json
{
  "result": "type"
}
```
**Validation:**
- [Validation rule 1]
- [Validation rule 2]

**Errors:**
| Code | When |
|------|------|
| [CODE] | [Condition] |

[Repeat for each RPC]

## Events (Server -> Client)

| Event | Payload | Recipients | Reliable |
|-------|---------|------------|----------|
| [event] | [data] | [who] | [Yes/No] |

### Event Definitions

#### [event_name]
**Purpose:** [What this event notifies]
**Triggered by:** [What causes this event]
**Payload:**
```json
{
  "field1": "type",
  "field2": "type"
}
```
**Recipients:** [All in session / Nearby / Specific players]

[Repeat for each event]

## Serialization

### Format Comparison
| Format | Message Size | Parse Speed | Debug-ability |
|--------|--------------|-------------|---------------|
| JSON | Baseline | Baseline | Excellent |
| MessagePack | 30-50% smaller | 2-3x faster | Moderate |
| Protobuf | 50-70% smaller | 5-10x faster | Requires tools |

### Recommended: [Format]
**Rationale:** [Why this format]

### Schema (if applicable)
```protobuf
[Schema definitions]
```

## Bandwidth Optimization

### Message Priority
| Priority | Types | Behavior |
|----------|-------|----------|
| Critical | [Types] | Always sent immediately |
| High | [Types] | Sent every update |
| Medium | [Types] | Batched, sent frequently |
| Low | [Types] | Sent when bandwidth allows |

### Compression
**Method:** [None / gzip / LZ4 / custom]
**Applied to:** [Which messages]
**Threshold:** [Compress if > X bytes]

### Batching
[How messages are batched for efficiency]

## Error Handling

### Error Codes
| Code | Category | Client Action |
|------|----------|---------------|
| [CODE] | [Category] | [What client should do] |

### Retry Policy
| Error Type | Retry | Backoff |
|------------|-------|---------|
| Transient | Yes | Exponential |
| Validation | No | N/A |
| Auth | Re-auth | N/A |
| Rate limit | Yes | Wait X seconds |

## Security

### Rate Limiting
| Method | Limit | Window | Penalty |
|--------|-------|--------|---------|
| [method] | [N] | [Xs] | [Action] |

### Input Validation
[What validation is performed on each RPC]

### Authentication Flow
```
[Authentication message sequence]
```

## Implementation Checklist
- [ ] Define message schemas
- [ ] Implement serialization
- [ ] Add authentication middleware
- [ ] Add rate limiting
- [ ] Implement each RPC handler
- [ ] Implement event broadcasting
- [ ] Add logging/metrics
- [ ] Test with simulated network conditions
```

Generate based on the user's game and communication requirements.
