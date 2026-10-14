# How to Update — IST

**Project:** `IST`
**Category:** CHIP_QUANTIZATION
**Domain:** chip quantization and model compression
**Date:** 2026-10-07

---

## Update Procedure

### Checking for Updates
```bash
IST --version
IST check-update
```

### Applying Updates
```bash
pip install --upgrade IST
```

### Rolling Back
```bash
pip install IST==<previous-version>
```

### Update Policy
- **Security updates:** Applied immediately
- **Feature updates:** Monthly release cycle
- **Breaking changes:** 6-month deprecation notice

## Verification

All 16 checks PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.
