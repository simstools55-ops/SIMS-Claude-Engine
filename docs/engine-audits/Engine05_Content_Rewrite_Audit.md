# Engine05 Content Rewrite Audit

## Purpose

Engine05 turns the analysis from earlier engines into actionable rewritten article content.

It must not decide the main query by itself. It consumes decisions from Engine01 to Engine04 and focuses on execution quality.

## Inputs

- Improvement_Request.md
- Main Query
- Primary Sub Queries
- Supporting Queries
- Search Intent Analysis
- Current H1 / Title / Description when available
- Current Article Body when provided
- Blog Profile
- Internal Link Candidates
- Knowledge Core and optional Knowledge Pack

## Outputs

Engine05 writes to the Improvement_Result sections:

- Revised Article Draft
- Revised Sections
- Added H2 / H3
- Added FAQ
- Added explanations
- Rewrite Summary
- Beginner Guide Notes

## Retain from Prototype

- Search intent first rewriting
- Do not rewrite for style only
- Preserve useful existing content
- Add missing sections only when needed
- Separate analysis from final publishing text

## Refactor for AI Exchange

Engine05 must accept structured AI Exchange input rather than free-form user instructions.

It must return structured output so SIMS can store the result and the user can paste changes into WordPress.

## Quality Gate

A rewrite passes Engine05 only if:

- It addresses the Main Query directly
- It incorporates important Sub Queries naturally
- It improves clarity for the reader
- It does not introduce unsupported facts
- It separates suggested metadata from body content
- It includes user-facing explanation of what changed

## Beginner Support

For non-expert users, Engine05 must explain:

- Which parts of the article should be replaced
- Which parts should be added
- Where the FAQ should be placed
- What should be copied into WordPress
- What should not be changed
