# How to Update — PODMAN

**Project:** `PODMAN`
**Category:** INFRA_DEVOPS
**Domain:** infrastructure and DevOps
**Date:** 2026-10-07

---

## Update Procedure

### Checking for Updates
```bash
PODMAN --version
PODMAN check-update
```

### Applying Updates
```bash
pip install --upgrade PODMAN
```

### Rolling Back
```bash
pip install PODMAN==<previous-version>
```

### Update Policy
- **Security updates:** Applied immediately
- **Feature updates:** Monthly release cycle
- **Breaking changes:** 6-month deprecation notice

## Verification

All 16 checks PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.
