# Data Model

## Core note types

| Type | Purpose |
|---|---|
| `system` | architecture, rules, invariants |
| `workflow` | repeatable process |
| `skill` | reusable capability |
| `project` | bounded outcome with context |
| `concept` | durable knowledge unit |
| `research` | evidence-backed investigation |
| `decision` | decision + rationale + alternatives |
| `learning` | reusable lesson |
| `error` | failure and root-cause record |
| `reference` | external/internal source pointer |
| `meeting` | discussion and outcomes |
| `person` | relationship/context note when useful |
| `area` | ongoing responsibility |
| `resource` | reusable asset |

## Recommended properties

```yaml
type: concept
status: draft
created: 2026-09-04
updated: 2026-09-04
source: 
confidence: 
owner: 
project: 
canonical: false
supersedes: 
superseded_by: 
tags: []
```

Use only properties that improve governance or retrieval. Avoid property bloat.

## Naming

Prefer stable, human-readable names. Use folders for broad system organization and links for relationships.
