---
name: incident-response
description: Generate incident response playbook
---

# Incident Response Playbook Generator

Generate a comprehensive incident response playbook for game operations.

## Context Gathering

Before generating, understand:

### Game Context
- Game type (live-service, multiplayer requirements)
- Critical systems (matchmaking, economy, progression)
- Player communication channels
- Revenue sensitivity

### Team Context
- Team structure and time zones
- On-call rotation exists?
- Communication tools (Slack, Discord, PagerDuty)

## Output Format

```markdown
# Incident Response Playbook: [Game Name]

## Severity Definitions

| Severity | Description | Response Time | Examples |
|----------|-------------|---------------|----------|
| SEV1 | Complete outage, data loss | < 15 min | Server down, exploit active |
| SEV2 | Major feature broken | < 1 hour | Matchmaking down, purchases failing |
| SEV3 | Significant degradation | < 4 hours | High latency, minor feature broken |
| SEV4 | Minor issue | Next business day | UI bug, cosmetic issue |

---

## Incident Command Structure

### Roles During Incident

| Role | Responsibility |
|------|----------------|
| **Incident Commander (IC)** | Coordinates response, makes decisions |
| **Technical Lead** | Diagnoses and fixes the issue |
| **Communications Lead** | Updates players and stakeholders |
| **Scribe** | Documents timeline and actions |

### Escalation Path

```
On-Call Engineer
      ↓ (10 min no response)
Team Lead
      ↓ (SEV1/SEV2)
Engineering Manager
      ↓ (SEV1 > 1 hour)
Director/VP
```

---

## Response Procedures

### SEV1: Critical Incident

#### Initial Response (0-15 min)
1. [ ] Acknowledge alert
2. [ ] Create incident channel: #incident-[date]-[brief]
3. [ ] Assign Incident Commander
4. [ ] Post initial status: "Investigating [symptom]"
5. [ ] Update status page to "Investigating"

#### Diagnosis (15-30 min)
1. [ ] Identify affected systems
2. [ ] Check recent deployments
3. [ ] Review error logs and metrics
4. [ ] Determine blast radius
5. [ ] Post findings to incident channel

#### Mitigation (30 min - 2h)
1. [ ] Decide: Rollback vs Fix Forward
2. [ ] Execute mitigation
3. [ ] Verify mitigation working
4. [ ] Update status: "Monitoring fix"
5. [ ] Communicate ETA to players

#### Resolution
1. [ ] Confirm issue resolved
2. [ ] Update status page: "Resolved"
3. [ ] Post player communication
4. [ ] Schedule postmortem (within 48h)

---

### SEV2: Major Incident

#### Initial Response (0-30 min)
1. [ ] Acknowledge and assess
2. [ ] Notify team lead
3. [ ] Create incident thread
4. [ ] Begin investigation

#### Resolution
1. [ ] Diagnose root cause
2. [ ] Implement fix
3. [ ] Verify resolution
4. [ ] Document for postmortem

---

## Common Scenarios

### Scenario: Server Outage
**Symptoms:** Players cannot connect, matchmaking fails
**Initial Checks:**
- Server health metrics
- Recent deployments
- Cloud provider status
- Network connectivity

**Common Causes:**
- Failed deployment
- Resource exhaustion
- Cloud provider incident
- DDoS attack

**Mitigation Options:**
1. Rollback recent deployment
2. Scale up resources
3. Failover to backup region
4. Enable DDoS protection

---

### Scenario: Database Performance
**Symptoms:** High latency, timeouts, failed queries
**Initial Checks:**
- Query performance
- Connection pool status
- Disk I/O
- Lock contention

**Common Causes:**
- Slow query
- Connection leak
- Disk full
- Missing index

**Mitigation Options:**
1. Kill problematic queries
2. Restart connection pools
3. Add capacity
4. Enable query result caching

---

### Scenario: Economy Exploit
**Symptoms:** Unusual currency generation, negative balances
**Initial Checks:**
- Transaction logs
- Player reports
- Unusual patterns
- Recent changes

**Immediate Actions:**
1. Disable affected feature
2. Identify affected accounts
3. Assess damage scope
4. Plan remediation

---

### Scenario: Authentication Failure
**Symptoms:** Players cannot log in
**Initial Checks:**
- Auth service health
- OAuth provider status
- Token validation
- Session storage

**Mitigation Options:**
1. Failover auth provider
2. Extend token expiry
3. Enable emergency bypass
4. Restart auth services

---

## Communication Templates

### Initial Acknowledgment
```
We're aware of an issue affecting [feature/service] and are
investigating. We'll provide updates as we learn more.
```

### Status Update
```
Update on [issue]: We've identified [cause] and are
[action being taken]. Estimated resolution: [time].
```

### Resolution Notice
```
The issue affecting [feature/service] has been resolved.
[Brief explanation]. Thank you for your patience.
```

### Compensation Announcement
```
To thank you for your patience during [issue], all players
will receive [compensation]. Check your [inbox/mail] in the
next [time].
```

---

## Post-Incident

### Postmortem Template
```markdown
## Incident Postmortem: [Title]

**Date:** [Date]
**Duration:** [Start - End]
**Severity:** [SEV level]
**Impact:** [Player/revenue impact]

### Timeline
[Chronological events]

### Root Cause
[What actually caused the issue]

### What Went Well
- [Positive item]

### What Could Be Improved
- [Improvement item]

### Action Items
| Action | Owner | Due Date |
|--------|-------|----------|
| [Action] | [Name] | [Date] |
```

### Follow-Up Checklist
- [ ] Postmortem written within 48 hours
- [ ] Postmortem reviewed with team
- [ ] Action items created and assigned
- [ ] Process improvements documented
- [ ] Communication reviewed for improvements

---

## Contacts

### Internal
| Role | Contact |
|------|---------|
| On-Call | [Phone/Pager] |
| Team Lead | [Contact] |
| Manager | [Contact] |

### External
| Provider | Support Contact |
|----------|----------------|
| Cloud Provider | [Contact] |
| Auth Provider | [Contact] |
| Payment Provider | [Contact] |
```

Generate the playbook customized for the specific game and team context provided.
