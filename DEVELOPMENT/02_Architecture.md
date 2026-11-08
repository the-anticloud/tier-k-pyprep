# Architecture — K_PYPREP

**Company:** Anticloud FZ LLE

## Overview

K_PYPREP is packaged as a single Anticloud binary with embedded PAX L5 Narrow L2 General 27B inference via llama.cpp.

## Components

| Component | Description |
| --- | --- |
| Core Engine | Upstream functionality |
| PAX Adapter | llama.cpp bridge for local AI |
| AIOSS Module | Append-only audit ledger |
| Crypto Layer | AES-256 encryption at rest |
| CLI | Unified command interface |

## Deployment

Single binary. No Docker, no Kubernetes, no cloud account.
