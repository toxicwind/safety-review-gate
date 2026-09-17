# Backfill 2026-09-17 — B2/C2 shards

Run-ID backfill for the safety-review gate investigation ledger.

- `shard-b2-20260917.txt` — 1,710 rows, md5 e17c3d2025255df2e23aa59341e905f1
- `shard-c2-20260917.txt` — 2,223 rows, md5 d90ae62cdd2d3b187492dc6bdc7ca80f
- `progress-b2c2-20260917-v3.tsv` — full progress log with defect disclosures
- `validation_report.json` — machine-readable validation results

Verification: 22/22 pages byte-exact vs live DB via order-aware checksums.
Full union A(4,621) + B_frozen(5,220) + C_frozen(2,760) + B2(1,710) + C2(2,223)
= 16,534 unique UUIDs, zero overlap across all 10 shard pairs.
