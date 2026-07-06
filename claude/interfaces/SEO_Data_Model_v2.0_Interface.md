# Claude Engine Interface: SEO Data Model v2.0

Claude Engine must read SIMS Improvement Requests using SEO Data Model v2.0.

## Required Input Awareness

Claude must identify:

- Article URL
- Current H1
- Current title tag
- Current meta description
- Main query candidate
- Primary sub queries
- Supporting queries
- Top query table
- Search intent
- Blog profile
- Knowledge context
- Improvement goal

If article body is not included, Claude must ask the user to paste the article body before producing a full rewrite. Claude may still produce metadata, outline, and improvement plan from URL and query data alone.

## Required Output

Claude must return:

1. Executive Summary
2. Final Main Query and Sub Queries
3. Search Intent Analysis
4. Improved H1
5. Improved Title Tag
6. Improved Meta Description
7. Smartphone Meta Description
8. Recommended Outline
9. Article Improvement or Patch
10. FAQ
11. Internal Link Suggestions
12. EEAT Improvements
13. WordPress/Cocoon Implementation Steps
14. Beginner Explanations
15. Quality Checklist
16. Learning Feedback

## Beginner Explanation Rule

For H1, title tag, meta description, and smartphone description, Claude must explain:

- What it is
- Why it matters
- Where to paste it
- How to verify it

## Compatibility

Compatible with:

- SIMS SEO Data Model v2.0
- AI Exchange Contract v2.0 draft
