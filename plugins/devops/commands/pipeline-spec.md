---
name: pipeline-spec
description: Generate a CI/CD pipeline specification for a game project
---

# CI/CD Pipeline Specification Generator

Generate a comprehensive CI/CD pipeline specification tailored to the project's needs.

## Context Gathering

Before generating, understand:

### Project Context
- Game engine (Unity/Unreal/Godot/Custom)
- Target platforms (PC, Console, Mobile, Web)
- Repository structure (monorepo, multi-repo)
- Team size and workflow (trunk-based, git flow)

### CI Platform
- GitHub Actions, GitLab CI, Jenkins, Azure DevOps, etc.
- Runner availability (hosted vs self-hosted)
- Budget constraints

### Current State
- Existing CI/CD (if any)
- Pain points to address
- Build time targets

## Output Format

```markdown
# CI/CD Pipeline Specification: [Project Name]

## Overview
**CI Platform:** [Platform]
**Engine:** [Engine]
**Platforms:** [Target platforms]
**Workflow:** [Branching strategy]

## Pipeline Triggers

| Event | Pipeline | Purpose |
|-------|----------|---------|
| Push to main | Full build + deploy | Production releases |
| Pull request | Quick build + tests | PR validation |
| Tag v*.*.* | Release pipeline | Version releases |
| Schedule (nightly) | Full test suite | Comprehensive testing |
| Manual | Deploy to [env] | On-demand deployment |

## Pipeline Stages

### Stage 1: Validation
**Duration:** ~2-3 minutes
**Runs on:** [Runner type]
```yaml
steps:
  - lint
  - format-check
  - license-check
```

### Stage 2: Build
**Duration:** ~[X] minutes
**Runs on:** [Runner type]

#### Platform Matrix
| Platform | Runner | Artifacts |
|----------|--------|-----------|
| Windows | windows-latest | game-win64.zip |
| macOS | macos-latest | game-osx.dmg |
| Linux | ubuntu-latest | game-linux.tar.gz |
| WebGL | ubuntu-latest | game-webgl.zip |

### Stage 3: Test
**Duration:** ~[X] minutes
```yaml
parallel:
  - unit-tests
  - integration-tests
```

### Stage 4: Deploy
**Environments:** [dev, staging, production]
```yaml
conditions:
  - dev: auto on develop
  - staging: auto on main
  - production: manual approval
```

## Caching Strategy

| Cache | Key Pattern | Size Estimate |
|-------|-------------|---------------|
| Unity Library | unity-${{ hashFiles('**/Packages/') }} | ~2GB |
| node_modules | npm-${{ hashFiles('**/package-lock.json') }} | ~500MB |

## Secrets Required

| Secret | Purpose | Scope |
|--------|---------|-------|
| STEAM_USERNAME | Steam deployment | deploy jobs |
| SIGNING_CERT | Code signing | build jobs |

## Environment Configuration

| Environment | URL | Protection |
|-------------|-----|------------|
| Development | dev.example.com | None |
| Staging | staging.example.com | None |
| Production | example.com | Required reviewers |

## Performance Targets

| Metric | Target |
|--------|--------|
| PR feedback | < 10 minutes |
| Full build | < 30 minutes |
| Deploy time | < 5 minutes |

## Estimated Costs

| Resource | Monthly Estimate |
|----------|------------------|
| CI minutes | $[X] |
| Storage | $[X] |
| Runners | $[X] |
```

Generate the pipeline specification based on the project context provided.
