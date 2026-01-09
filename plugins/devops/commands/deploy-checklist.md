---
name: deploy-checklist
description: Generate deployment checklist for a release
---

# Deployment Checklist Generator

Generate a comprehensive deployment checklist tailored to the release type and platform.

## Context Gathering

Before generating, understand:

### Release Context
- Release type (major, minor, patch, hotfix)
- Target platforms (Steam, Console, Mobile, Web)
- New features or changes included
- Database migrations required

### Team Context
- Release owner
- On-call personnel
- Communication channels

## Output Format

```markdown
# Deployment Checklist: v[Version]

## Release Overview
**Version:** [X.Y.Z]
**Type:** [Major/Minor/Patch/Hotfix]
**Date:** [Scheduled date/time UTC]
**Owner:** [Name]
**On-Call:** [Name]

---

## Pre-Deployment (T-24h to T-1h)

### Code Readiness
- [ ] All features merged to release branch
- [ ] Code freeze in effect
- [ ] No critical bugs in release
- [ ] Release notes drafted

### QA Sign-Off
- [ ] Smoke tests passed
- [ ] Regression tests passed
- [ ] Platform-specific tests passed
- [ ] QA lead has signed off

### Build Readiness
- [ ] Release build created
- [ ] Build version matches release
- [ ] Artifact stored and accessible
- [ ] Build tested on target platforms

### Database
- [ ] Migrations tested on staging
- [ ] Rollback scripts prepared
- [ ] Backup scheduled
- [ ] Data integrity verified

### Feature Flags
- [ ] New features flagged OFF by default
- [ ] Flag configurations reviewed
- [ ] Rollback flags identified

### Communication
- [ ] Team notified of deployment window
- [ ] Support team briefed on changes
- [ ] Player announcement drafted
- [ ] Status page ready

---

## Deployment (T-0)

### Start Deployment
- [ ] Announce deployment starting in #releases
- [ ] Set status page to "Deploying"
- [ ] Begin deployment procedure

### Platform-Specific

#### Steam
- [ ] Upload to Steam depot
- [ ] Set build live on branch
- [ ] Verify SteamDB shows update
- [ ] Wait for CDN propagation (~15 min)

#### Console (if applicable)
- [ ] Certification passed
- [ ] Submit to platform
- [ ] Coordinate regional timing

#### Mobile (if applicable)
- [ ] iOS: Submit for review or release
- [ ] Android: Set rollout percentage
- [ ] Monitor for review issues

#### Web (if applicable)
- [ ] Deploy to CDN
- [ ] Invalidate cache
- [ ] Verify version endpoint

### Database Migrations
- [ ] Run migrations
- [ ] Verify migration success
- [ ] Spot-check data integrity

### Feature Flag Activation
- [ ] Enable flags per rollout plan
- [ ] Verify flag states

---

## Post-Deployment (T+0 to T+4h)

### Immediate Verification
- [ ] Application starts successfully
- [ ] Login flow works
- [ ] Core gameplay functional
- [ ] No error spikes in logs

### Metrics Check
- [ ] Error rate normal (< [X]%)
- [ ] Latency normal (< [X]ms)
- [ ] Player count recovering
- [ ] No crash spikes

### Smoke Test
- [ ] New player flow
- [ ] Returning player flow
- [ ] Purchase flow (if applicable)
- [ ] Key features working

### Communication
- [ ] Update status page to "Deployed"
- [ ] Announce deployment complete
- [ ] Publish patch notes
- [ ] Notify support team

---

## Monitoring Period (T+4h to T+24h)

### Extended Monitoring
- [ ] Review error logs
- [ ] Check player feedback channels
- [ ] Monitor support tickets
- [ ] Watch revenue metrics (if applicable)

### Issue Triage
- [ ] Assess any reported issues
- [ ] Determine if hotfix needed
- [ ] Document known issues

---

## Rollback Procedure (If Needed)

### Triggers for Rollback
- Crash rate > [X]%
- Error rate > [X]%
- Revenue impact > [X]%
- Critical exploit discovered

### Rollback Steps
1. [ ] Announce rollback in #incidents
2. [ ] Disable new feature flags
3. [ ] Deploy previous version
4. [ ] Verify rollback successful
5. [ ] Update status page
6. [ ] Communicate to players
7. [ ] Schedule postmortem

---

## Sign-Off

### Deployment Complete
- [ ] All verification passed
- [ ] Monitoring shows stable
- [ ] Release owner sign-off
- [ ] Handoff to on-call complete

### Post-Deployment
- [ ] Update release log
- [ ] Close deployment ticket
- [ ] Schedule retrospective (if issues)
```

Generate the checklist customized for the specific release details provided.
