# Exchange Processor Engine

## Purpose

Convert a SIMS `Improvement_Request.md` into a complete article improvement package.

## Input Sections to Read

- Article information
- Search Console snapshot
- Main query candidate
- Sub query candidates
- Top queries table
- Current metadata
- Improvement goal
- Required outputs

## Processing Steps

1. Confirm target article and search intent.
2. Validate main query and sub query candidates.
3. Identify content gaps from query data.
4. Generate recommended SEO metadata.
5. Generate article improvement instructions.
6. Generate beginner-friendly explanation.
7. Return standardized result files.

## Main Query Handling

Default rule:

- Accept SIMS main query candidate unless evidence suggests a better target.

Override conditions:

- Candidate has weak relevance to article.
- Candidate has low search intent fit.
- Candidate is too broad for the current article.
- Another query has stronger ranking opportunity.

When overriding, clearly report:

- Original candidate
- Selected query
- Reason
