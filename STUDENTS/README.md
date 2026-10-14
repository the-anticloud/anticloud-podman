# Students — PODMAN

**Project:** PODMAN  
**Category:** INFRA_DEVOPS  
**Upstream:** see BENCH.json  
**Pinned commit:** `3f04d208a3964d0e16d6d7b995c0ae30bf9fe38d`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d640c491902d42bdbc275866b8b700c3bdc1f1dcbb28e63bf85651f52efdfe12`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `3f04d208a3964d0e16d6d7b995c0ae30bf9fe38d`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `d640c491902d42bdbc275866b8b700c3bdc1f1dcbb28e63bf85651f52efdfe12`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
