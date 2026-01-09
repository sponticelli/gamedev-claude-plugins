---
name: infra-plan
description: Generate infrastructure architecture plan
---

# Infrastructure Architecture Plan Generator

Generate a comprehensive infrastructure architecture plan for a game project.

## Context Gathering

Before generating, understand:

### Game Requirements
- Game type (single-player, multiplayer, live-service)
- Expected concurrent users (CCU)
- Real-time requirements (latency sensitivity)
- Data storage needs (player profiles, leaderboards, etc.)

### Technical Context
- Preferred cloud provider (AWS, GCP, Azure)
- Budget constraints
- Team ops experience
- Existing infrastructure (if any)

### Geographic Requirements
- Primary player regions
- Data residency requirements
- CDN needs

## Output Format

```markdown
# Infrastructure Architecture: [Project Name]

## Overview
**Game Type:** [Type]
**Cloud Provider:** [Provider]
**Target CCU:** [Number]
**Primary Region:** [Region]

## Architecture Diagram

```
[ASCII diagram of infrastructure]
```

## Components

### Compute Layer
| Component | Service | Specs | Quantity | Purpose |
|-----------|---------|-------|----------|---------|
| Game servers | [Service] | [Size] | [N] | Game logic |
| API servers | [Service] | [Size] | [N] | REST API |

### Data Layer
| Data Type | Service | Configuration | Purpose |
|-----------|---------|---------------|---------|
| Player profiles | [DB] | [Config] | Account data |
| Game state | [DB] | [Config] | Match data |
| Analytics | [DB] | [Config] | Telemetry |

### Supporting Services
| Service | Provider | Purpose |
|---------|----------|---------|
| Matchmaking | [Service] | Player matching |
| CDN | [Service] | Asset delivery |
| Auth | [Service] | Authentication |

## Scaling Strategy

### Auto-Scaling Rules
| Trigger | Action | Cooldown |
|---------|--------|----------|
| CCU > [N] | Add [N] servers | [Time] |
| CCU < [N] | Remove [N] servers | [Time] |
| CPU > [%] | Scale up | [Time] |

### Capacity Tiers
| Tier | CCU Range | Servers | Est. Cost/Month |
|------|-----------|---------|-----------------|
| Quiet | 0-1K | [N] | $[X] |
| Normal | 1K-10K | [N] | $[X] |
| Peak | 10K-50K | [N] | $[X] |
| Event | 50K+ | [N] | $[X] |

## Regional Distribution

| Region | Purpose | Services | Latency Target |
|--------|---------|----------|----------------|
| [Region] | Primary | All | <50ms |
| [Region] | Secondary | Game servers | <80ms |

## Cost Estimate

### Monthly Baseline
| Category | Service | Estimate |
|----------|---------|----------|
| Compute | [Service] | $[X] |
| Database | [Service] | $[X] |
| Network | [Service] | $[X] |
| Storage | [Service] | $[X] |
| **Total** | | **$[X]** |

### Launch Surge
**Duration:** [Time]
**Multiplier:** [X]x baseline
**Budget:** $[X]

## High Availability

### Redundancy
| Component | Strategy | RPO | RTO |
|-----------|----------|-----|-----|
| Database | Multi-AZ | 0 | <1 min |
| Game servers | Auto-replace | N/A | <2 min |
| API | Load balanced | N/A | <30 sec |

### Disaster Recovery
| Scenario | Response | Recovery Time |
|----------|----------|---------------|
| AZ failure | Failover | < 5 minutes |
| Region failure | DNS failover | < 15 minutes |
| Data corruption | Point-in-time | < 1 hour |

## Security

### Network Security
- VPC isolation
- Security groups
- Private subnets for databases

### Application Security
- TLS everywhere
- API authentication
- Rate limiting

### Data Security
- Encryption at rest
- Encryption in transit
- Regular backups

## Monitoring

### Metrics
| Metric | Alert Threshold | Response |
|--------|-----------------|----------|
| Server CPU | > 80% | Scale up |
| Error rate | > 1% | Investigate |
| Latency p95 | > 100ms | Investigate |

### Dashboards
- Player CCU
- Server health
- Error rates
- Latency percentiles

## Implementation Phases

### Phase 1: MVP
- Single region
- Basic scaling
- Managed services

### Phase 2: Production
- Multi-AZ
- Auto-scaling
- Monitoring

### Phase 3: Global
- Multi-region
- CDN
- Advanced DR
```

Generate the infrastructure plan based on the project context provided.
