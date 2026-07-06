# Engine04 AI Exchange Quality Contract

## Purpose

Define how Engine04 receives AI Exchange-compatible inputs and returns a structured SEO quality audit for downstream engines.

## Inputs

### Required

- Article URL
- Main query candidate
- Primary sub queries
- Search Console query table, if available
- Engine03 primary search intent
- Engine03 user need hierarchy

### Optional

- Current H1
- Current title tag
- Current meta description
- Article body
- Blog Profile
- Knowledge Pack
- Internal link candidates

## Output sections

Engine04 must output these sections:

1. Gate Status
2. SEO Quality Audit
3. Metadata Audit
4. Heading Structure Audit
5. Content Completeness Audit
6. EEAT Audit
7. Beginner Usability Audit
8. Internal Link Opportunity Audit
9. Risk Notes
10. Decision
11. Handoff to Engine05

## Decision values

- `GO`
- `REVISE_ANALYSIS`
- `STOP`

## Quality rule

Engine04 may identify deficiencies, but it must not produce final improved text. Deficiencies are passed to Engine05 and later rewrite engines.
