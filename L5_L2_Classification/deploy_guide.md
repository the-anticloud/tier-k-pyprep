# Deploy Guide — K_PYPREP
**Tier:** TIER_7_BIOSIGNALS_NEURO | **Stack:** Python 3.11, pyprep 0.x, mne 1.7+, numpy, PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, pyprep 0.4+, mne 1.7+. CPU for PREP. GPU optional for PAX.

## Environment
8GB RAM. CPU for PREP pipeline (30-90s per recording). GPU for PAX quality evaluation.

## AIOSS Integration
```bash
aioss init --module K_PYPREP --output ./k_pyprep.aioss
aioss append --chain ./k_pyprep.aioss --payload ./output.bin --module K_PYPREP
aioss verify --chain ./k_pyprep.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="K_PYPREP",
    aioss_chain="./K_PYPREP.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./K_PYPREP.aioss --verbose
python -m K_PYPREP.tests.smoke
```
