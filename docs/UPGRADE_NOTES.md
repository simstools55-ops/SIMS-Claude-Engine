# Claude Engine Upgrade Notes for AI Exchange v1.0

## What changes

Claude Engine now treats SIMS input as an improvement case, not a casual prompt.

## Required behavior

- Return structured result files.
- Include SEO metadata every time.
- Include beginner explanations.
- Include WordPress application guidance.
- Preserve measurable outputs for SIMS tracking.

## Quality Check

Before returning a result, confirm:

- Main query is present.
- Sub queries are present.
- H1 is present.
- Title tag is present.
- Meta description is present.
- Smartphone description is present.
- User checklist is present.
