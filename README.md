# Budgeted Evidence Reuse for Typed-Walk Filtering

This repository provides the recorded measurements behind the paper. The request traces, timing summaries, and cache diagnostics let readers examine when reusing graph traversal results saves time and when checking or evicting cached entries adds work.

The [measurement downloads](https://github.com/LiCHOLjq/budgeted-evidence-reuse-data/releases/tag/measurements) are grouped by experiment:

| Collection | What it contains |
| --- | --- |
| Main experiment (13 ZIPs) | Request traces and diagnostics for comparing execution policies across workloads and memory budgets. |
| Threshold experiment (1 ZIP) | Measurements from varying the threshold used to construct cached evidence. |
| Earlier experiments (3 ZIPs) | Ablation, comparison, and replication runs. |

To reproduce the main results, start in the [code repository](https://github.com/LiCHOLjq/budgeted-evidence-reuse-code) and run `python tools/fetch_main.py` from its root. The script downloads, verifies, and extracts all 13 main archives. For manual downloads, the [data guide](DATA.md) lists the files for each collection, and the [manifest](manifest.json) gives their sizes and SHA-256 checksums.
