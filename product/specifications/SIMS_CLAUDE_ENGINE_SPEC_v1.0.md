# SIMS Claude Engine Specification v1.0

## Purpose

SIMS Claude Engine defines the Claude-side article improvement layer separated from SIMS Core.

## Boundaries

### Claude Engine does

- Improve articles
- Interpret Search Console queries
- Generate WordPress-ready content
- Produce Improvement Result reports
- Suggest next improvement actions

### Claude Engine does not

- Connect to Search Console
- Manage spreadsheets
- Schedule improvements
- Measure post-improvement performance directly
- Deploy GitHub Pages

## Interface

The primary interface is AI Exchange:

- `Improvement_Request.md`
- `Improvement_Result.md`
- `Measurement_Report.md`
- `Improvement_Feedback.md`

## Versioning

Claude Engine versions are independent from SIMS Core versions.

Example:

- SIMS Core v5.0
- SIMS Claude Engine v1.0

## Upgrade Policy

Article improvement quality should be improved by changing Claude Engine files, not by changing SIMS Core.
