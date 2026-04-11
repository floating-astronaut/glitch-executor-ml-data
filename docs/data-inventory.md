# Data Inventory

Current extracted dataset inventory for the private Glitch ML data repository.

## Summary

- Approximate size: `880.44 MB`
- Top-level sources:
  - `viper`
  - `cobra`
  - `taipan`
  - `mamba`
  - `anaconda`
  - `hydra`
  - `king_cobra`
  - `terciopelo`
- Research sources:
  - `research/hydra`
  - `research/king_cobra_pro_modules`

## File Counts

- `ml_data/viper`: `28` files
- `ml_data/cobra`: `20` files
- `ml_data/taipan`: `22` files
- `ml_data/taipan/archive_19col`: `2` files
- `ml_data/mamba`: `19` files
- `ml_data/anaconda`: `28` files
- `ml_data/hydra`: `10` files
- `ml_data/king_cobra/training`: `8` files
- `ml_data/king_cobra/auto_trades`: `17` files
- `ml_data/king_cobra/assistant`: `20` files
- `ml_data/terciopelo/resolutions`: `60` files

## Notes

- `terciopelo` is represented by closed-trade resolution JSON files rather than the same CSV schema used by the snake bots.
- `king_cobra` is split into `training`, `auto_trades`, and `assistant` datasets.
- `taipan` includes an `archive_19col` folder for the older schema variant.
- `research/hydra` contains indicator backtests, multitimeframe experiments, merged XAU research datasets, and retrain reports.
- `research/king_cobra_pro_modules` contains combined all-bot datasets, manifests, and BTC research exports from the King Cobra research pipeline.
- `research/king_cobra_pro_modules/btc_combined_all_bots.csv` was split into `btc_combined_all_bots_parts/` to stay within normal GitHub file-size limits without relying on Git LFS.
