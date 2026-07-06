# Engine03 AI Exchange Search Intent Contract

## Engine name

Engine03 Search Intent / User Needs Analysis Engine

## Input contract

Engine03 consumes:

```markdown
# SIMS Improvement Request v1.0
```

Required sections:

- Article URL
- Main Query Candidate
- Primary Sub Queries
- Supporting Queries
- Search Console Snapshot
- Engine02 Search Console Analysis Result

Optional sections:

- Current H1
- Current Title Tag
- Current Meta Description
- Article Body
- Blog Profile
- Dynamic Knowledge

## Output contract

Engine03 writes to `Improvement_Result.md` under:

```markdown
## Engine03 Search Intent Analysis
```

Required fields:

- Gate Status
- Primary Search Intent
- Secondary Search Intents
- Intent Group Table
- User Need Hierarchy
- User Situation
- User Pain Point
- Expected Answer
- Missing Context
- Beginner Explanation
- Handoff to Engine04

## Intent group taxonomy

Use these labels when possible:

- Know: wants explanation or definition.
- Do: wants procedure or action.
- Troubleshooting: wants cause and fix.
- Compare: wants comparison or selection.
- Transactional: wants product, service, price, or purchase decision.
- Local: wants location-specific information.
- Navigational: wants a specific site, service, or page.
- Mixed: multiple strong intents exist.

## Handoff rule

Engine03 must produce a compact brief for Engine04. Engine04 uses it to audit whether the current article satisfies the primary and secondary search intents.
