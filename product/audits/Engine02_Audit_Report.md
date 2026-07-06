# Engine02 Audit Report

## Source reviewed

Prototype file:

```text
SIMSv2/engine02.md
```

## Prototype role

Engine02 is defined as **Search Console Analysis Engine**.

Its purpose is to analyze Google Search Console data and determine the improvement priority and improvement direction for the target article.

## Evaluation

### Keep

The separation is architecturally correct.

Engine02 should only analyze Search Console data. It should not analyze search intent, competitors, SERPs, rewrite content, generate titles, create FAQ, or recommend internal links.

This boundary is important because SIMS now supplies Search Console data directly, while later engines interpret intent, strategy, rewrite, metadata, and publishing.

### Modify

The input model must be updated from manual top 10 queries to AI Exchange input.

Old input:

- Main keyword
- Article URL
- Search Console top 10 queries
- Clicks
- Impressions
- CTR
- Average position

New input:

- Normalized intake from Engine01
- Main query candidate
- Primary sub query candidates
- Supporting query table, recommended max 20
- Clicks
- Impressions
- CTR
- Position
- Device and country when available
- Date range
- Optional improvement history

### Preserve prototype judgment model

The prototype's three judgment types should be preserved:

1. Article quality is generally good; minor updates may improve results.
2. Search intent mismatch is suspected; search intent analysis is required.
3. Major improvement is required, including structure and metadata review.

### Do not change

Engine02 must continue to avoid:

- Search intent conclusions
- Competitor analysis
- SERP analysis
- Article rewriting
- H1 / title / description generation
- FAQ recommendation
- Internal link recommendation
- Publishing decisions

Those belong to later engines.

## Final decision

Engine02 remains **Search Console Analysis Engine**.

It receives normalized data from Engine01 and outputs a Search Console analysis summary, priority query set, and improvement judgment for downstream engines.
