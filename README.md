# Reproducibility materials

These materials accompany “Correction under conflicting evidence in retrieval-augmented systems: A three-gate evaluation” submitted to Web Intelligence. The repository contains publication-level aggregate results, figure-generation code, and the six figures used in the manuscript and supplement.

## Contents

- `analysis/`: derived aggregate JSON used by the plotting scripts.
- `scripts/`: publication-level plotting code.
- `figures/`: the final figure PDFs embedded in the submitted documents.

## Run

Use Python 3.11 or later. From the repository root:

```bash
python -m pip install -r requirements.txt
python scripts/make_journal_figures.py
python scripts/make_followup_figures.py
```

The scripts write additional diagnostic plates to `figures_revision/` and tables to `tables/`. The files in `figures/` are the final editorial figure versions; the scripts generate related diagnostic plates from the saved aggregate results.

## Scope

This is a publication-level package. It does not contain API credentials, raw model responses, retrieved web passages, licensed benchmark images, or the original experiment result tree. Consequently, it supports inspection of the reported aggregates and regeneration of the included diagnostic plots, but not rerunning model calls or recomputing all aggregates from raw responses. Some analyses require third-party benchmark assets and service access. No human validation is claimed for the automatic semantic audit.

