# SIMS Claude Engine v2.0.5 - Engine04 SEO Quality Audit

This package advances Claude Engine v2 development from Engine03 Search Intent Analysis to Engine04 SEO Quality Audit.

Engine04 is preserved from the operational prototype as the **SEO Quality Audit Engine**. Its responsibility is to audit whether the current improvement direction is safe, coherent, and SEO-quality-ready before rewrite or patch creation begins. It must not rewrite the article, create titles, create metadata, add FAQ, or generate publishing output.

## What changed

- Preserved the proven prototype principle: Engine04 is an audit engine, not a rewrite engine.
- Updated input to receive `Improvement_Request.md`, Engine01 intake output, Engine02 Search Console analysis, and Engine03 Search Intent analysis.
- Added AI Exchange v1.0 compatibility.
- Standardized audit gates: intent match, H1/title alignment, heading structure, content completeness, EEAT, readability, internal-link opportunity, and beginner usability.
- Added explicit `go / revise / stop` decision for downstream Engine05.
- Added beginner-friendly audit explanation requirements.

## Repository target

Upload this package into the `SIMS-Claude-Engine` repository.

Recommended commit message:

```text
Add Engine04 SEO Quality audit and AI Exchange refactor
```
