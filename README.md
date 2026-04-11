# Glitch ML Data

Private ML data repository for the Glitch Executor ecosystem.

This repo is intended to hold the accumulated training data, labeled outcomes, and research datasets behind the Glitch trading stack. It is not a public repo and should remain private.

## Purpose

This repository exists to:

- preserve irreplaceable historical ML data
- centralize bot-specific CSV and JSON outcome datasets
- preserve research datasets and merged experiment outputs
- make future data drops easy to append in one place
- keep research data separate from the public code repositories

## Privacy Rule

This repository must remain private.

Do not publish it, mirror it, or copy it into any public Glitch repository.

## Current Dataset

- Bots included: `viper`, `cobra`, `taipan`, `mamba`, `anaconda`, `hydra`, `king_cobra`, `terciopelo`
- Approximate current size: `880.44 MB`
- Research snapshots included under `research/` for Hydra and King Cobra
- Schema notes: [docs/ml_schema_comparison.md](./docs/ml_schema_comparison.md)
- Inventory: [docs/data-inventory.md](./docs/data-inventory.md)

## Structure

```text
glitch-ml-data-private/
|-- ml_data/
|   |-- viper/
|   |-- cobra/
|   |-- taipan/
|   |-- mamba/
|   |-- anaconda/
|   |-- hydra/
|   |-- king_cobra/
|   `-- terciopelo/
|-- research/
|   |-- hydra/
|   `-- king_cobra_pro_modules/
`-- docs/
```

## Future Data Drops

When adding new data:

- keep the existing bot folder names stable
- preserve original filenames when possible
- add only data files, not environments or logs
- keep secrets, credentials, and broker state out of this repo
- update [docs/data-inventory.md](./docs/data-inventory.md) if the structure changes materially

## Relationship To Public Repos

The public Glitch repositories expose the architecture and strategy layer.

This private repo holds the data moat behind that work:

- labeled trade outcomes
- ML training CSVs
- assistant signal logs
- resolution JSON histories
- research merges and experimental dataset exports

If this dataset is ever shared externally, it should be done deliberately and by maintainer decision only.
