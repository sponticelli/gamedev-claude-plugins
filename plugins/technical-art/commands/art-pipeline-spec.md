---
name: art-pipeline-spec
description: Generate an art production pipeline specification
---

# Art Pipeline Specification Generator

Create a comprehensive art pipeline specification document.

## Context Gathering

Before generating the pipeline spec, understand the project:

### Analyze Art Requirements
- What types of assets are needed?
- What DCC tools does the team use?
- What's the target engine?
- What's the team size and experience?

### Understand Technical Requirements
- What platforms are targeted?
- What are the performance budgets?
- What file formats are required?
- What version control is used?

### Check Existing Infrastructure
- Is there an existing pipeline to build on?
- What automation exists?
- What pain points exist currently?
- What tools/scripts are available?

### Identify Constraints
- Timeline for pipeline development?
- Team resources for pipeline work?
- Budget for tools/licenses?
- Technical limitations?

Use this context to design appropriate pipeline.

## Output Format

```markdown
# Art Pipeline Specification: [Project Name]

## Overview
**Asset types covered:** [What this pipeline handles]
**DCC tools:** [Software used]
**Target engine:** [Destination]
**Team size:** [Number of artists]

## Pipeline Diagram

```
[DCC] → [Export] → [Process] → [Import] → [Engine]
         ↓           ↓           ↓
     [Validate]  [Optimize]  [Verify]
```

## Directory Structure

### Source (Art Repo)
```
/Art
├─ /Characters
├─ /Environment
├─ /Props
├─ /VFX
└─ /UI
```

### Intermediate
[Where exports go before engine import]

### Engine Assets
[Final asset locations in engine project]

## Naming Conventions

| Asset Type | Pattern | Example |
|------------|---------|---------|
| [Type] | [Pattern] | [Example] |

## Per-Asset Workflows

### [Asset Type]
**Source format:** [.blend, .psd, etc.]
**Export format:** [.fbx, .png, etc.]
**Engine format:** [prefab, asset, etc.]

#### Workflow Steps
1. [Step 1]
2. [Step 2]
3. [Step 3]

#### Validation Rules
| Rule | Check | Error Handling |
|------|-------|----------------|
| [Rule] | [What's checked] | [What happens on fail] |

[Repeat for each asset type]

## Automation

### Export Scripts
| Script | Purpose | Trigger |
|--------|---------|---------|
| [Name] | [What it does] | [When it runs] |

### Import Automation
| Processor | Asset Types | Actions |
|-----------|-------------|---------|
| [Name] | [What it handles] | [What it does] |

### CI/CD Integration
[How pipeline integrates with builds]

## Quality Assurance

### Automated Checks
| Check | When | Pass Criteria |
|-------|------|---------------|
| [Check] | [Export/Import/Build] | [Requirements] |

### Manual Review
[What requires human review]

## Troubleshooting

| Issue | Cause | Solution |
|-------|-------|----------|
| [Problem] | [Why] | [Fix] |

## Maintenance

### Documentation
[Where docs are kept, how updated]

### Training
[How artists learn the pipeline]

### Feedback
[How issues are reported and addressed]
```

Generate based on the user's project and pipeline needs.
