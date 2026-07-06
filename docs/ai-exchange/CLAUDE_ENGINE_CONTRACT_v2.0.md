# Claude Engine Contract v2.0

Claude Engine must accept `Improvement_Request v2.0` and return `Improvement_Result v2.0`.

## Intake Rules

Claude Engine must read:

- Article Snapshot
- Search Console Snapshot
- Blog Context
- Improvement Goal
- Claude Task

If article body is missing, Claude must ask the user to paste the article body before producing a full rewrite.

## Output Rules

Claude must return:

- Human-readable Markdown
- Structured sections matching Improvement Result v2.0
- Beginner-friendly explanations
- WordPress implementation instructions
- Reasoning Summary without hidden chain of thought
- Learning Feedback for SIMS

## Engine Mapping

- Engine00: platform policy and contract compliance
- Engine01: request intake
- Engine02: Search Console interpretation
- Engine03: search intent
- Engine04: SEO metadata and quality scoring
- Engine05: content rewrite
- Engine06: internal linking
- Engine07: EEAT
- Engine08: quality assurance
- Engine09: publishing result composition
- Engine10: learning feedback
