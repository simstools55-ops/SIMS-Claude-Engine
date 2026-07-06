# Engine02 AI Exchange Search Console Contract

## Engine

```text
Engine ID: E02
Engine Name: Search Console Analysis Engine
Role: Search Console data analysis and improvement priority judgment
```

## Primary input

Engine02 receives `Engine01 Intake Result` and the normalized Search Console query table from SIMS AI Exchange.

## Required fields

- Request ID
- Article URL
- Date range
- Main query candidate
- Query table with at least:
  - Query
  - Clicks
  - Impressions
  - CTR
  - Position

## Recommended fields

- Primary sub queries, 3 to 5
- Supporting queries, up to 15
- Total query table size, max 20
- Device data, if available
- Country data, if available
- Previous measurement data, if available

## Analysis dimensions

Engine02 analyzes each query using:

- Search demand: impressions
- Current traction: clicks
- CTR opportunity: low CTR relative to position
- Ranking opportunity: positions 5 to 20 are high-priority opportunities
- Query stability: repeated appearance in Search Console data when available
- Main query consistency: whether the query supports the candidate main query

## Priority rules

Recommended priority order:

1. High impressions
2. Position 5 to 20
3. Low CTR
4. Meaningfully related to the article topic
5. Useful for the user's improvement goal

## Judgment types

Engine02 returns one of:

```text
JUDGMENT_1_MINOR_UPDATE
JUDGMENT_2_INTENT_REVIEW_REQUIRED
JUDGMENT_3_MAJOR_REWRITE_REQUIRED
```

## Output object

```text
SearchConsole_Analysis_Result
├── Request_Metadata
├── Query_Opportunity_Table
├── Priority_Query_Set
├── CTR_Opportunity
├── Position_Opportunity
├── Improvement_Judgment
├── Improvement_Rationale
└── Ready_For_Next_Engine
```

## Beginner explanation requirement

Engine02 must explain the meaning of its judgment in plain language.

Example:

```text
この記事は表示回数があるのにクリック率が低いため、検索結果で選ばれにくい状態です。ただし、本文修正ではなく、次のEngineで検索意図とタイトルの確認が必要です。
```

## Prohibited outputs

Engine02 must not output:

- Final H1
- Final title tag
- Final meta description
- Rewritten article body
- FAQ text
- Internal link anchors
- SERP conclusions
