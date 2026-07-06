# SIMS Claude Engine v2.0.4 - Engine03 Search Intent Audit

This package advances Claude Engine v2 development from Engine02 Search Console Analysis to Engine03 Search Intent Analysis.

Engine03 is preserved from the operational prototype as the **Search Intent / User Needs Analysis Engine**. Its responsibility is to convert query data and Google evaluation signals into structured user intent. It must not rewrite the article, generate metadata, propose internal links, or create publishing output.

## What changed

- Preserved the proven prototype principle: analyze the searcher, not only the keyword.
- Updated input to receive `Improvement_Request.md`, Engine01 intake output, and Engine02 Search Console analysis.
- Added AI Exchange v1.0 compatibility.
- Standardized intent groups: Know, Do, Compare, Troubleshooting, Transactional, Local, Navigational.
- Added beginner-friendly explanation requirements.
- Added explicit handoff to Engine04 SEO Audit.

## Repository target

Upload this package into the `SIMS-Claude-Engine` repository.

Recommended commit message:

```text
Add Engine03 Search Intent audit and AI Exchange refactor
```
