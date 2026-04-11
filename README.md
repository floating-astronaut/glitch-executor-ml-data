# Glitch Executor ML Data

Private ML data repository for the Glitch Executor ecosystem.

This repository holds the raw and cleaned datasets behind the Glitch trading stack: training exports, labeled outcomes, merged research snapshots, and bot-level data that should stay separate from both public code and trained-model artifacts.

## Repo Role

This repo is the data layer for the Glitch trading family. It exists to preserve:

- raw bot-level ML datasets
- cleaned dataset variants
- research-only data drops
- labeled outcomes and merged experiment exports
- schema and inventory documentation

## What Lives Here

- `ml_data/` for primary bot-level datasets
- `ml_data_clean/` for cleaned or normalized derivatives
- `research/` for experiment snapshots and exploratory exports
- `docs/` for inventories and schema notes

## Privacy

This repository must remain private.

Do not mirror it to a public repo. Do not commit credentials, broker state, or environment secrets. If any subset is ever shared externally, it should be done deliberately and by maintainer decision only.

## Relationship To Other Repos

- public Glitch repos expose architecture and strategy code
- `glitch-executor-ml-data` stores the raw and cleaned training-data layer
- `glitch-executor-ml-models` stores the trained artifact layer derived from this data

## Working Notes

When adding new data:

- keep bot folder names stable where possible
- preserve source filenames unless normalization requires a new derivative
- document structural changes in `docs/`
- avoid disposable runtime noise, logs, and caches
