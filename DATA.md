# Measurement data

Download the ZIP archives from the [measurements release](https://github.com/LiCHOLjq/budgeted-evidence-reuse-data/releases/tag/measurements). Check the archive sizes and SHA-256 values against [the manifest](manifest.json). For analysis commands and a downloader for the main experiment, see the [code repository](https://github.com/LiCHOLjq/budgeted-evidence-reuse-code).

| Collection | Archives | Accepted request executions |
| --- | --- | ---: |
| Main experiment | `measurements-main-part01.zip` through `measurements-main-part13.zip` | 5,999,680 |
| Threshold experiment | `measurements-threshold.zip` | 172,800 |
| Ablation, comparison and replication experiments | `measurements-historical-part01.zip` through `measurements-historical-part03.zip` | 1,867,200 |

Extract the archives for each desired collection into the same code checkout. The main experiment spans thirteen independent ZIPs and the historical collection spans three. Each ZIP contains distinct files. Extract all parts of a collection to restore it. The `release-data/` directory contains the coverage notes and individual file checksums for each collection.

The main experiment includes 5,193,600 primary, 76,800 observer-control and 729,280 diagnostic executions. The files also document an interrupted attempt with 3,072 requests, which is excluded from the reported counts. Repeated measurements can share queries and workloads. The adaptive-gate inventory records an untimed replay.
