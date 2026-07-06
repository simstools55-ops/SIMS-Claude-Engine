# Engine03 Audit Report

## Prototype source

- Source: `ai-yoshida-main/SIMS/Engine3`
- Prototype name: `検索意図・ユーザーニーズ分析エンジン`
- Prototype role: Analyze the searcher, not the keyword.

## Preserve

Engine03 must preserve these proven ideas:

1. Search keywords and search intent are different.
2. Different queries may belong to the same user need.
3. The engine must identify what the searcher truly wants to solve.
4. The engine must not rewrite or improve the article directly.
5. The output must be handed to later engines as structured intent.

## Refactor for SIMS v2

### Previous input

- Main keyword
- Article URL
- Search Console top queries
- Engine02 Google evaluation analysis

### New input

- `Improvement_Request.md`
- Engine01 normalized intake
- Engine02 Search Console analysis result
- Main Query Candidate
- Primary Sub Queries
- Supporting Queries, recommended max 20
- Current H1, title tag, meta description if available
- Optional article body
- Optional Blog Profile

## New responsibility boundary

Engine03 may:

- Group queries by user intent.
- Identify primary user need.
- Identify secondary user needs.
- Identify missing user context.
- Explain why the intent matters.

Engine03 must not:

- Rewrite the article.
- Generate H1, title tag, or description.
- Add FAQ.
- Decide internal links.
- Produce final publishable content.

## Quality gate

Engine03 passes only when it outputs:

- Primary search intent.
- Intent group map.
- User situation.
- User pain point.
- Expected answer.
- Urgency level.
- Handoff notes for Engine04.
