# Engine04 - SEO Quality Audit Engine v2

## Engine ID
E04

## Role
Engine04 audits the quality and safety of the improvement direction before article rewriting begins.

Engine04 does not write, rewrite, patch, publish, or generate final SEO metadata. It only audits whether the article can be improved under the current intent and data assumptions.

## Required Inputs

- `Improvement_Request.md`
- Engine01 intake output
- Engine02 Search Console analysis output
- Engine03 Search Intent analysis output
- Article body, if supplied by the user
- Current H1 / title tag / meta description, if supplied
- Blog Profile / Knowledge Pack, if supplied

## Core Audit Gates

### Gate 1: Search intent alignment
Confirm whether the proposed improvement direction matches the primary user need identified by Engine03.

### Gate 2: H1, title, and description alignment
Audit whether the current H1, title tag, and meta description are aligned with the main query and expected answer.

### Gate 3: Heading structure
Audit whether H2/H3 structure can answer the search intent in a logical order.

### Gate 4: Content completeness
Identify missing information, duplicate information, unnecessary information, and information that should be clarified.

### Gate 5: EEAT
Audit whether the article has sufficient experience, expertise, authoritativeness, trustworthiness, caution notes, and practical evidence.

### Gate 6: Readability and beginner usability
Audit whether a beginner can understand what to do next without needing specialist knowledge.

### Gate 7: Internal link opportunity
Audit whether internal links are likely needed, but do not create final link placement. Pass opportunities to later engines.

## Decision Output

Engine04 must output exactly one decision:

- `GO`: Improvement can proceed to Engine05.
- `REVISE_ANALYSIS`: Engine03 or previous analysis needs correction.
- `STOP`: The request lacks enough data to proceed safely.

## Prohibited Actions

Engine04 must not:

- Rewrite article text
- Generate final H1/title/meta description
- Create FAQ content
- Add internal links
- Produce publishing output
- Create final improvement patches

## Output Destination

Engine04 output is handed off to Engine05.
