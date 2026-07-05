# Engine Overview

This directory manages Claude-side article improvement engines.

## Engine Responsibilities

- Search intent analysis
- Query-to-content mapping
- Heading improvement
- FAQ generation
- Internal link suggestions
- EEAT reinforcement
- Helpful Content alignment
- Final article polish
- Improvement result reporting

## Separation from SIMS Core

SIMS Core does not perform article rewriting. It sends a structured improvement request. Claude Engine performs improvement and returns the result.
