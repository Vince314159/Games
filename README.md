# RIB — Roblox Investment Banking

RIB is a research dashboard for screening Roblox experiences using structured public-market signals, evidence maturity, model outputs, and validation records.

## Dashboard

The site is a static, client-side dashboard. No synthetic game metrics are bundled into the production build.

Use **Load Sheet CSVs** to import CSV exports from the RIB data system:

- 1 Market Discovery
- 2 RIB Score
- 3 Signal Analysis
- 4 Validation

The importer auto-detects each export, joins records by game name, preserves missing/unknown evidence, and distinguishes legacy v1 scoring from current v2.4 status.

## Data integrity

- Missing evidence stays missing; it is not silently converted to zero.
- Provisional or unscored v2.4 records are labeled as such.
- Legacy v1 scores are never presented as final v2.4 scores.
- Imported CSV contents remain in the user's browser/local storage and are not committed to this repository.
- Roblox imagery is visual/reference context and is separated from RIB scoring evidence.

## Purpose

Built for the RIB DECA Innovation Plan research project. RIB is a diligence-prioritization and research system, not financial advice or an automatic acquisition decision engine.

## Run locally

Open `index.html` in a modern browser. No build step or server is required.