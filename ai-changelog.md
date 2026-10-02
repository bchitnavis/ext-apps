# AI Changelog

## 2026-10-02 - Commit outstanding working-tree changes and ignore generated artifacts

- Reviewed every repository under `repos` in one pass and committed the work that had accumulated in this one but was never recorded. The changes below were made in earlier sessions; this entry records them rather than claiming them as new work.
- Modified: `.gitignore`, `examples/pdf-server/main.ts`.
- Added: `ext-apps.code-workspace`.
- Extended [.gitignore](.gitignore) to exclude data files (`*.csv`, `*.xlsx`, `*.parquet`, `*.db`, `*.duckdb` and similar), `.env` files, and generated artifacts (`__pycache__`, `.venv`, `node_modules`, `dist`, `build`, and .NET `bin`/`obj`). Rules only affect files that are not already tracked, so nothing was untracked and nothing was deleted.
