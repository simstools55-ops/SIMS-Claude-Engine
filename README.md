# SIMS Claude Engine v2.0.2 - Engine01 Intake Audit

This package advances Claude Engine v2 development from Engine00 Platform Policy to Engine01 Project Intake.

Engine01 is not the Search Intent engine. The prototype defines Engine01 as the **Project Intake Engine**. This role is preserved because it is architecturally sound: Engine01 validates, normalizes, and prepares the request before later engines perform search intent, SERP, rewrite, metadata, QA, and publishing work.

## What changed

- Preserved the proven prototype responsibility of Engine01.
- Updated Engine01 to accept SIMS AI Exchange `Improvement_Request` as the primary input.
- Expanded Search Console handling from top 10 queries to recommended top 20 queries.
- Added SEO metadata fields required for v5 workflows: H1, title tag, meta description, smartphone description.
- Added explicit beginner-safety rules: Engine01 must not analyze, rewrite, or invent missing data.
- Added a normalized intake object that downstream engines can consume consistently.

## Repository target

Upload this package into the `SIMS-Claude-Engine` repository.

Recommended commit message:

```text
Add Engine01 intake audit and AI Exchange refactor
```
