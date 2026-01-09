---
name: server-scaling-plan
description: Generate a server infrastructure and scaling strategy for a multiplayer game
---

# Server Scaling Plan Generator

Create a server infrastructure and scaling strategy document.

## Context Gathering

Before generating the scaling plan, understand the infrastructure needs:

### Analyze Player Projections
- Expected concurrent users at launch?
- Growth projections over time?
- Peak vs average player ratios?
- Geographic distribution of players?

### Understand Session Model
- Players per session/server?
- Average session duration?
- Persistent or match-based?
- What happens during off-peak hours?

### Check Technical Requirements
- What compute resources per session? (CPU, memory)
- What's the tick rate?
- Bandwidth per player?
- Any special hardware needs? (GPU compute, etc.)

### Identify Constraints
- Budget range for hosting?
- Cloud provider preferences/requirements?
- Compliance requirements? (GDPR, regional data)
- Team expertise level with infrastructure?

Use this context to plan appropriate infrastructure and scaling.

## Output Format

```markdown
# Server Scaling Plan: [Game Name]

## Executive Summary
**Hosting Approach:** [Managed / Self-hosted / Hybrid]
**Primary Provider:** [AWS / GCP / Azure / Other]
**Launch Regions:** [Regions]
**Monthly Cost Estimate:** [Range]

## Capacity Model

### Player Projections
| Timeframe | CCU | Peak CCU | Sessions |
|-----------|-----|----------|----------|
| Launch | [X] | [Y] | [Z] |
| Month 3 | [X] | [Y] | [Z] |
| Year 1 | [X] | [Y] | [Z] |

### Resource Requirements
| Resource | Per Session | At Launch Peak | At Scale Peak |
|----------|-------------|----------------|---------------|
| CPU cores | [X] | [Y] | [Z] |
| Memory (GB) | [X] | [Y] | [Z] |
| Bandwidth (Mbps) | [X] | [Y] | [Z] |

### Instance Planning
| Instance Type | Purpose | Count (Launch) | Count (Scale) |
|---------------|---------|----------------|---------------|
| [Type] | [Purpose] | [N] | [N] |

## Regional Deployment

| Region | Provider Zone | Priority | Capacity |
|--------|---------------|----------|----------|
| [Region] | [Zone] | [P1/P2/P3] | [X instances] |

**Latency targets:**
- Same region: <50ms
- Adjacent region: <100ms
- Fallback region: <200ms

## Scaling Strategy

### Reactive Scaling
| Trigger | Condition | Action | Cooldown |
|---------|-----------|--------|----------|
| High load | CPU > 70% for 5m | +2 instances | 10m |
| Queue depth | Wait > 30s | +4 instances | 5m |
| Low load | CPU < 30% for 15m | -1 instance | 20m |

### Predictive Scaling
[Pattern-based pre-scaling approach]

### Warm Pool
**Size:** [X% spare capacity]
**Warm-up time:** [Xm to ready]

### Cost Controls
**Max instances:** [N]
**Budget alerts:** [Thresholds]

## Cost Breakdown

### Launch Estimate (Monthly)
| Component | Cost |
|-----------|------|
| Game servers (compute) | $X |
| Backend services | $X |
| Database | $X |
| Bandwidth | $X |
| Matchmaking/services | $X |
| **Total** | **$X** |

### At Scale Estimate (Monthly)
| Component | Cost |
|-----------|------|
| [Same breakdown] | $X |
| **Total** | **$X** |

### Optimization Opportunities
- [Opportunity 1]: [Savings estimate]
- [Opportunity 2]: [Savings estimate]

## Deployment Strategy
**Method:** [Blue-Green / Rolling / Canary]
**Rollback time:** [Xm]
**Zero-downtime:** [Yes/No]

## Monitoring & Alerts

### Key Metrics
| Metric | Warning | Critical |
|--------|---------|----------|
| Match wait time | >30s | >60s |
| Instance CPU | >70% | >90% |
| Error rate | >1% | >5% |
| Available capacity | <20% | <10% |

## Disaster Recovery
**Backup frequency:** [X]
**Recovery time objective:** [Xm]
**Recovery point objective:** [Xm]

## Next Steps
1. [Immediate action]
2. [Setup task]
3. [Validation task]
```

Generate based on the user's game and infrastructure requirements.
