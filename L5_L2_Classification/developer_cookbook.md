# Developer Cookbook — K_PYPREP
**Stack:** Python 3.11, pyprep 0.x, mne 1.7+, numpy, PAX 27B, AIOSS_FORMAT
**Domain:** PyPREP: automated EEG preprocessing pipeline for Anticloud clinical data

## Preprocess EEG with PREP
```python
from k_pyprep import PREPPipeline

pipeline = PREPPipeline(
    pax_model="./pax-27b-q4.gguf",
    aioss_chain="./pyprep.aioss"
)

raw = mne.io.read_raw_edf("./patient_001.edf", preload=True)
result = pipeline.run(
    raw=raw,
    line_freqs=[50],  # EU line noise
    montage="standard_1020"
)
print(f"Bad channels removed: {result.bad_channels}")
print(f"Data quality: {result.quality_score:.2f}")
print(f"PAX assessment: {result.pax_assessment}")
print(f"Chain: {result.chain_hash}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
