# Educators — PODMAN

**Project:** PODMAN  
**Category:** INFRA_DEVOPS  
**Upstream:** see BENCH.json  
**Pinned commit:** `3f04d208a3964d0e16d6d7b995c0ae30bf9fe38d`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d640c491902d42bdbc275866b8b700c3bdc1f1dcbb28e63bf85651f52efdfe12`  
**Date:** October 2026

## Teaching with PODMAN

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `d640c491902d42bdbc275866b8b700c3bdc1f1dcbb28e63bf85651f52efdfe12` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
