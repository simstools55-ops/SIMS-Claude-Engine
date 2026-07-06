# SIMS Claude Engine v2.0.3 - Engine02 Search Console Audit

This package advances Claude Engine v2 development from Engine01 Project Intake to Engine02 Search Console Analysis.

Engine02 is preserved as the **Search Console Analysis Engine** from the operational prototype. Its responsibility is to analyze the Search Console snapshot prepared by Engine01 and decide improvement priority and direction. It must not perform search intent analysis, SERP analysis, rewriting, metadata generation, FAQ creation, or internal link recommendations.

## What changed

- Preserved the proven prototype responsibility of Engine02.
- Updated input from manual top 10 queries to SIMS AI Exchange top query set, recommended max 20 rows.
- Defined query scoring using impressions, clicks, CTR, position, and improvement opportunity.
- Preserved the three improvement judgments from the prototype.
- Added AI Exchange output section for downstream engines.
- Added beginner-safe rules so Engine02 explains what the numbers mean without generating article changes.

## Repository target

Upload this package into the `SIMS-Claude-Engine` repository.

Recommended commit message:

```text
Add Engine02 Search Console audit and AI Exchange refactor
```
