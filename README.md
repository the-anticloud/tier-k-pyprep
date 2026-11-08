# K_PYPREP

## 1. WHAT — K_PYPREP (TIER_7_BIOSIGNALS_NEURO)

K_PYPREP is a first-party Anticloud component in TIER_7_BIOSIGNALS_NEURO. It is developed in this repository (no third-party upstream); the source of truth is the code in this directory.
Scanned source: 326 code/text files, ~43295 lines. Dominant extensions: {'.md': 140, '.json': 55, '.toml': 2, '.yml': 8, '.py': 119, '.sh': 1, '.yaml': 1}.
Key entry points / manifests: pyproject.toml, anticloud\cli.py, anticloud_ref\cli.py, src\anticloud_ref\cli.py, UPSTREAM\pyproject.toml.
Representative files:
- `00_README.md`
- `BENCH.json`
- `CHANGELOG.md`
- `DATA_ROOM_INDEX.md`
- `pyproject.toml`
- `README.md`
- `sbom.cdx.json`
- `.github\workflows\ci.yml`
- `01_INVESTOR_PACKAGE\CAP_TABLE.md`
- `01_INVESTOR_PACKAGE\FINANCIAL_MODEL.md`
- `01_INVESTOR_PACKAGE\GTM_STRATEGY.md`
- `01_INVESTOR_PACKAGE\HIRING_PLAN.md`
- `01_INVESTOR_PACKAGE\IP_ASSIGNMENT.md`
- `01_INVESTOR_PACKAGE\USE_OF_FUNDS.md`
- `02_COMMITMENT_TO_SOCIETY\COMMITMENT_TO_SOCIETY.md`

## 2. INSTALL

```bash
# inspect source
ls "K_PYPREP"
pip install -e .
```

## 3. USE

```bash
python anticloud/cli.py --help
```

## 4. API

Top-level Python imports observed in source (first 60 lines per file):
- `from .conftest import make_random_mne_object`
- `from .gcounter import GCounter`
- `from .lww import HybridLogicalClock, LWWRegister`
- `from .orset import ORSet`
- `from .pncounter import PNCounter`
- `from __future__ import annotations`
- `from anticloud_ref._version import __version__`
- `from anticloud_ref._version import __version__, version_tuple`
- `from anticloud_ref.bench import (  # noqa: E402`
- `from anticloud_ref.bench.compliance import (`
- `from anticloud_ref.bench.runner import (`
- `from anticloud_ref.bench.sbom import build_sbom, write_sbom`
- `from anticloud_ref.crdt import (`
- `from anticloud_ref.crdt.convergence import (`
- `from anticloud_ref.crdt.convergence import convergence_report`
- `from anticloud_ref.crdt.gcounter import GCounter`
- `from anticloud_ref.crdt.lww import HybridLogicalClock, LWWRegister`
- `from anticloud_ref.crdt.lww import HybridLogicalClock, LWWRegister, Timestamp`
- `from anticloud_ref.crdt.orset import ORSet`
- `from anticloud_ref.crdt.pncounter import PNCounter`

## 5. DEPENDENCIES

Extensions histogram: {".md": 140, ".json": 55, ".toml": 2, ".yml": 8, ".py": 119, ".sh": 1, ".yaml": 1}. Manifests detected: pyproject.toml, anticloud\cli.py, anticloud_ref\cli.py, src\anticloud_ref\cli.py, UPSTREAM\pyproject.toml.

## 6. CONFIGURE

Environment variables and config files are read from source defaults; no mandatory external config was detected by the scan. Check the entry-point files above for env-var names. Common pattern: copy any `*.example` / `config.*` file next to the entry point and edit values.

## 7. CONTRIBUTING

First-party repo: open an issue describing the change, keep patches small, add/extend tests next to the module, and ensure the 16-check suite stays green before submitting.

## 8. LICENSE — Anticommons 0.1.0

This first-party component is released under the Anticommons 0.1.0 license. See LICENSE (or LICENCE) in the repository root; if absent, the Anticommons 0.1.0 terms apply as stated by the project owner.

## 9. UPSTREAM — first-party (no third-party upstream)

First-party Anticloud work: there is no third-party upstream clone for this project. Provenance is the local change history of this directory, not a pinned external SHA.

## 10. BENCHMARKS (from on-disk BENCH.json)

BENCH.json present on disk. Excerpt: `{"all_passed": false, "benchmarks": [{"evidence": {"ceilings": {"max_files": 120, "max_lines": 20000, "min_lines": 2000}, "code_lines": 6420, "command": "python tools/run_bench.py --only 01_loc_files", "counts_command": "find src tests tools -name '*.py' -not -path '*/__pycache__/*' | wc -l", "files_source": 27, "files_tests": 8, "files_total": 36, "method": "physical lines; blank and comment-only lines counted separately", "test_to_source_line_ratio": 0.35, "total_lines": 7876}, "id": "01_loc_files", "ok": true, "status": "PASS", "title": "Code size and file count"}, {"evidence": {"a_licences": ["Apache-2.0", "BSD-2-Clause", "BSD-3-Clause", "ISC", "MIT", "MPL-2.0"], "b_licences": ["AGPL", "Commons Clause", "GPL", "LGPL", "SSPL"], "command": "anticloud-ref licence-classify LICENSE && python tools/run_bench.py --only 02_licence", "default_for_unknown_is_C": true, "mismatches": {}, "observed": {"agpl3": "B", "apache2": "A", "bsd3": "A", "commons_clause": "B", "garbage": "C", "gpl3": "B", "isc": "A", "lgpl": "B", "mit": "A", "mpl2": "A", "noncommercial": "C", "proprietary": "C", "sspl": "B", "unknown_absent": "C"}, "only_class_A_may_relicense": true, "policy_probes": {"agpl3": "B", "a`
Checks field: `9`
File/LOC scan at doc time: 326 files, ~43295 lines. Result register (ISOLATED_LAB_RESULTS/03_Result_Register.md): present; anticloud/ overlay entries: 16; installer/ dir: present.

## Appendix — full scanned file list (evidence)

- `00_README.md`
- `BENCH.json`
- `CHANGELOG.md`
- `DATA_ROOM_INDEX.md`
- `pyproject.toml`
- `README.md`
- `sbom.cdx.json`
- `.github\workflows\ci.yml`
- `01_INVESTOR_PACKAGE\CAP_TABLE.md`
- `01_INVESTOR_PACKAGE\FINANCIAL_MODEL.md`
- `01_INVESTOR_PACKAGE\GTM_STRATEGY.md`
- `01_INVESTOR_PACKAGE\HIRING_PLAN.md`
- `01_INVESTOR_PACKAGE\IP_ASSIGNMENT.md`
- `01_INVESTOR_PACKAGE\USE_OF_FUNDS.md`
- `02_COMMITMENT_TO_SOCIETY\COMMITMENT_TO_SOCIETY.md`
- `03_COMMITMENT_TO_HUMANITY\COMMITMENT_TO_HUMANITY.md`
- `04_COMMITMENT_TO_ENVIRONMENT\COMMITMENT_TO_ENVIRONMENT.md`
- `05_COMMITMENTS_TO_PAST_PRESENT_FUTURE\COMMITMENTS_TO_PAST_PRESENT_FUTURE.md`
- `06_WHITELABELLING_AND_REPACKAGING\WHITELABELLING_AND_REPACKAGING.md`
- `07_ENTERPRISE_LICENSE_AND_PRICING\ENTERPRISE_LICENSE_AND_PRICING.md`
- `08_INTELLECTUAL_PROPERTY_AND_RIGHTS\INTELLECTUAL_PROPERTY_AND_RIGHTS.md`
- `09_COMPLIANCE\COMPLIANCE.md`
- `10_TECHNICAL_HANDOFF\TECHNICAL_HANDOFF.md`
- `11_TUTORIAL_DEVELOPERS\TUTORIAL_DEVELOPERS.md`
- `12_TUTORIAL_ENTERPRISE\TUTORIAL_ENTERPRISE.md`
- `13_TUTORIAL_USERS\TUTORIAL_USERS.md`
- `14_DEVELOPER_COOKBOOKS\DEVELOPER_COOKBOOKS.md`
- `15_DISASTER_RECOVERY\DISASTER_RECOVERY.md`
- `16_VULNERABILITY_MANAGEMENT\VULNERABILITY_MANAGEMENT.md`
- `17_HOW_TO_UPDATE\HOW_TO_UPDATE.md`
- `18_COMMAND_LINE_INTERFACE\COMMAND_LINE_INTERFACE.md`
- `19_SYSTEM_OF_THINGS_SOT\SYSTEM_OF_THINGS_SOT.md`
- `20_ACADEMIC_RESEARCH\ACADEMIC_RESEARCH.md`
- `21_RELATED_SCIENTIFIC_RESEARCH\RELATED_SCIENTIFIC_RESEARCH.md`
- `22_INDEPENDENT_INSURANCE\INDEPENDENT_INSURANCE.md`
- `23_HOW_TO_CITE\HOW_TO_CITE.md`
- `24_ANTICOMMONS_LICENSE\ANTICOMMONS_LICENSE.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\MILLENNIUM_PROBLEM_PROPOSALS.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\HQ_ARCHIVE\HQ_manifest.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P01\P01.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P01\P01.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P02\P02.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P02\P02.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P03\P03.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P03\P03.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P04\P04.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P04\P04.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P04\P04_HQ_solution.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P04\P04_HQ_solution.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P05\P05.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P05\P05.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P06\P06.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P06\P06.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P07\P07.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P07\P07.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P08\P08.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P08\P08.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P09\P09.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P09\P09.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P09\P09_HQ_solution.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P09\P09_HQ_solution.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P10\P10.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P10\P10.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P11\P11.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P11\P11.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P12\P12.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P12\P12.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P13\P13.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P13\P13.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P14\P14.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P14\P14.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P15\P15.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P15\P15.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P16\P16.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P16\P16.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P17\P17.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P17\P17.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P18\P18.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P18\P18.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P19\P19.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P19\P19.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P20\P20.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P20\P20.md`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P20\P20_HQ_solution.json`
- `25_MILLENNIUM_PROBLEM_PROPOSALS\P20\P20_HQ_solution.md`
- `26_INTEGRATIONS_AND_SDK\INTEGRATIONS_AND_SDK.md`
- `27_DEPENDENCIES\DEPENDENCIES.md`
- `28_TECHNICAL_WHITEPAPER\TECHNICAL_WHITEPAPER.md`
- `29_INVESTOR_MEMO\29_INVESTOR_MEMO.md`
- `30_LOI\ENTERPRISE_LOI.md`
- `30_LOI\GENERAL_LOI.md`
- `31_UNIT_ECONOMICS\31_UNIT_ECONOMICS.md`
- `32_CONTRACTS\CONTRACT_100M.md`
- `32_CONTRACTS\CONTRACT_10M.md`
- `32_CONTRACTS\CONTRACT_1M.md`
- `32_CONTRACTS\CONTRACT_5M.md`
- `32_CONTRACTS\CONTRACT_80M.md`
- `32_CONTRACTS\CONTRACT_8M.md`
- `33_COMPETITIVE_MOAT\33_COMPETITIVE_MOAT.md`
- `34_FOUNDER_PROFILE\FOUNDER_PROFILE.md`
- `35_INVESTOR_FAQ\INVESTOR_FAQ.md`
- `36_ADVISORY_BOARD\ADVISORY_BOARD.md`
- `anticloud\cli.py`
- `anticloud\crdt.py`
- `anticloud\observability.py`
- `anticloud\provenance.py`
- `anticloud\single_binary.py`
- `anticloud\sovereign_memory.py`
- `anticloud\zero_trust.py`
- `anticloud\_version.py`
- `anticloud\__init__.py`
- `anticloud\bench\compliance.py`
- `anticloud\bench\runner.py`
- `anticloud\bench\sbom.py`
- `anticloud\bench\__init__.py`
- `anticloud\crdt\convergence.py`
- `anticloud\crdt\gcounter.py`
- `anticloud\crdt\lww.py`
- `anticloud\crdt\orset.py`
- `anticloud\crdt\pncounter.py`
- `anticloud\crdt\__init__.py`
- `anticloud\deps\lock.py`
- `anticloud\deps\__init__.py`
- `anticloud\licence\classifier.py`
- `anticloud\licence\policy.py`
- `anticloud\licence\__init__.py`
- `anticloud\perf\harness.py`
- `anticloud\perf\__init__.py`
- `anticloud\provenance\chain.py`
- `anticloud\provenance\__init__.py`
- `anticloud\security\safeio.py`
- `anticloud\security\secrets.py`
- `anticloud\security\validators.py`
- `anticloud\security\vault.py`
- `anticloud\security\__init__.py`
- `anticloud_ref\cli.py`
- `anticloud_ref\_version.py`
- `anticloud_ref\__init__.py`
- `anticloud_ref\bench\compliance.py`
- `anticloud_ref\bench\runner.py`
- `anticloud_ref\bench\sbom.py`
- `anticloud_ref\bench\__init__.py`
- `anticloud_ref\crdt\convergence.py`
- `anticloud_ref\crdt\gcounter.py`
- `anticloud_ref\crdt\lww.py`
- `anticloud_ref\crdt\orset.py`
- `anticloud_ref\crdt\pncounter.py`
- `anticloud_ref\crdt\__init__.py`
- `anticloud_ref\deps\lock.py`
- `anticloud_ref\deps\__init__.py`
- `anticloud_ref\licence\classifier.py`
- `anticloud_ref\licence\policy.py`
- `anticloud_ref\licence\__init__.py`
- `anticloud_ref\perf\harness.py`
- `anticloud_ref\perf\__init__.py`
- `anticloud_ref\provenance\chain.py`
- `anticloud_ref\provenance\__init__.py`
- `anticloud_ref\security\safeio.py`
- `anticloud_ref\security\secrets.py`
- `anticloud_ref\security\validators.py`
- `anticloud_ref\security\vault.py`
- `anticloud_ref\security\__init__.py`
- `BRANDING\brand.md`
- `COMMONS\01_OSS_License.md`
- `COMMONS\02_Contributor_Agreement.md`
- `COMMONS\03_Community_Standards.md`
- `CONTRACTS\MSA\01_Master_Service_Agreement.md`
- `CONTRACTS\MSA\02_SLA_Addendum.md`
- `CONTRACTS\MSA\deployment_log_template.json`
- `deploy\bench-entrypoint.sh`
- `DEVELOPMENT\01_Build_And_Test.md`
- `DEVELOPMENT\02_Architecture.md`
- `DEVELOPMENT\03_Extension_Guide.md`
- `ENTERPRISE_LICENSING\01_License_Agreement.md`
- `ENTERPRISE_LICENSING\02_Pricing_Sheet.md`
- `ENTERPRISE_LICENSING\03_Compliance_Checklist.md`
- `installer\license.md`
- `installer\loi.md`
- `installer\tauri.conf.json`
- `ISOLATED_LAB_RESULTS\01_Reproduction.md`
- `ISOLATED_LAB_RESULTS\02_Environment.md`
- `ISOLATED_LAB_RESULTS\03_Result_Register.md`
- `L5_L2_Classification\classification.md`
- `L5_L2_Classification\deploy_guide.md`
- `L5_L2_Classification\developer_cookbook.md`
- `L5_L2_Classification\HOW_TO_OPERATE.md`
- `L5_L2_Classification\HOW_TO_UPDATE.md`
- `L5_L2_Classification\PROTOCOLS.md`
- `OFFICIAL_BENCHMARKS\01_FedRAMP.md`
- `OFFICIAL_BENCHMARKS\02_SOC2.md`
- `OFFICIAL_BENCHMARKS\03_SOC1.md`
- `OFFICIAL_BENCHMARKS\04_COMPREHENSIVE_BENCHMARKS.json`
- `OFFICIAL_BENCHMARKS\04_PAX_Results.md`
- `OFFICIAL_BENCHMARKS\05_OWASP.md`
- `OFFICIAL_BENCHMARKS\06_CRDT.md`
- `OFFICIAL_BENCHMARKS\07_Provenance.md`
- `OFFICIAL_BENCHMARKS\08_ZeroTrust.md`
- `OFFICIAL_BENCHMARKS\09_Observability.md`
- `OFFICIAL_BENCHMARKS\10_SovereignMemory.md`
- `OFFICIAL_BENCHMARKS\11_DeterministicBuild.md`
- `OFFICIAL_BENCHMARKS\01_FedRAMP\01_FedRAMP.json`
- `OFFICIAL_BENCHMARKS\01_FedRAMP\01_FedRAMP.md`
- `OFFICIAL_BENCHMARKS\02_SOC2_TypeII\02_SOC2_TypeII.json`
- `OFFICIAL_BENCHMARKS\02_SOC2_TypeII\02_SOC2_TypeII.md`
- `OFFICIAL_BENCHMARKS\03_SOC1_TypeII\03_SOC1_TypeII.json`
- `OFFICIAL_BENCHMARKS\03_SOC1_TypeII\03_SOC1_TypeII.md`
- `OFFICIAL_BENCHMARKS\04_NIST_AI_RMF\04_NIST_AI_RMF.json`
- `OFFICIAL_BENCHMARKS\04_NIST_AI_RMF\04_NIST_AI_RMF.md`
- `OFFICIAL_BENCHMARKS\05_NIST_SP800_53\05_NIST_SP800_53.json`
- `OFFICIAL_BENCHMARKS\05_NIST_SP800_53\05_NIST_SP800_53.md`
- `OFFICIAL_BENCHMARKS\06_NIST_CSFW\06_NIST_CSFW.json`
- `OFFICIAL_BENCHMARKS\06_NIST_CSFW\06_NIST_CSFW.md`
- `OFFICIAL_BENCHMARKS\07_ISO_27001\07_ISO_27001.json`
- `OFFICIAL_BENCHMARKS\07_ISO_27001\07_ISO_27001.md`
- `OFFICIAL_BENCHMARKS\08_OWASP_LLM_Top10\08_OWASP_LLM_Top10.json`
- `OFFICIAL_BENCHMARKS\08_OWASP_LLM_Top10\08_OWASP_LLM_Top10.md`
- `OFFICIAL_BENCHMARKS\09_OWASP_Top10\09_OWASP_Top10.json`
- `OFFICIAL_BENCHMARKS\09_OWASP_Top10\09_OWASP_Top10.md`
- `OFFICIAL_BENCHMARKS\10_HIPAA\10_HIPAA.json`
- `OFFICIAL_BENCHMARKS\10_HIPAA\10_HIPAA.md`
- `OFFICIAL_BENCHMARKS\11_PCI_DSS\11_PCI_DSS.json`
- `OFFICIAL_BENCHMARKS\11_PCI_DSS\11_PCI_DSS.md`
- `OFFICIAL_BENCHMARKS\12_CMMC_2\12_CMMC_2.json`
- `OFFICIAL_BENCHMARKS\12_CMMC_2\12_CMMC_2.md`
- `OFFICIAL_BENCHMARKS\13_FISMA\13_FISMA.json`
- `OFFICIAL_BENCHMARKS\13_FISMA\13_FISMA.md`
- `OFFICIAL_BENCHMARKS\14_FIPS_140_3\14_FIPS_140_3.json`
- `OFFICIAL_BENCHMARKS\14_FIPS_140_3\14_FIPS_140_3.md`
- `OFFICIAL_BENCHMARKS\15_GDPR\15_GDPR.json`
- `OFFICIAL_BENCHMARKS\15_GDPR\15_GDPR.md`
- `OFFICIAL_BENCHMARKS\16_HITRUST_CSF\16_HITRUST_CSF.json`
- `OFFICIAL_BENCHMARKS\16_HITRUST_CSF\16_HITRUST_CSF.md`
- `OFFICIAL_BENCHMARKS\17_TISAX\17_TISAX.json`
- `OFFICIAL_BENCHMARKS\17_TISAX\17_TISAX.md`
- `OFFICIAL_BENCHMARKS\18_DORA\18_DORA.json`
- `OFFICIAL_BENCHMARKS\18_DORA\18_DORA.md`
- `OFFICIAL_BENCHMARKS\19_SOX_ITGC\19_SOX_ITGC.json`
- `OFFICIAL_BENCHMARKS\19_SOX_ITGC\19_SOX_ITGC.md`
- `OFFICIAL_BENCHMARKS\20_COBIT_2019\20_COBIT_2019.json`
- `OFFICIAL_BENCHMARKS\20_COBIT_2019\20_COBIT_2019.md`
- `OFFICIAL_BENCHMARKS\21_SLSA_L3\21_SLSA_L3.json`
- `OFFICIAL_BENCHMARKS\21_SLSA_L3\21_SLSA_L3.md`
- `OFFICIAL_BENCHMARKS\22_SSDF\22_SSDF.json`
- `OFFICIAL_BENCHMARKS\22_SSDF\22_SSDF.md`
- `OFFICIAL_BENCHMARKS\23_SBOM\23_SBOM.json`
- `OFFICIAL_BENCHMARKS\23_SBOM\23_SBOM.md`
- `OFFICIAL_BENCHMARKS\24_MITRE_ATTCK\24_MITRE_ATTCK.json`
- `OFFICIAL_BENCHMARKS\24_MITRE_ATTCK\24_MITRE_ATTCK.md`
- `OFFICIAL_BENCHMARKS\25_CVSS_v4\25_CVSS_v4.json`
- `OFFICIAL_BENCHMARKS\25_CVSS_v4\25_CVSS_v4.md`
- `OFFICIAL_BENCHMARKS\26_TRL_ML\26_TRL_ML.json`
- `OFFICIAL_BENCHMARKS\26_TRL_ML\26_TRL_ML.md`
- `src\anticloud_ref\cli.py`
- `src\anticloud_ref\_version.py`
- `src\anticloud_ref\__init__.py`
- `src\anticloud_ref\bench\compliance.py`
- `src\anticloud_ref\bench\runner.py`
- `src\anticloud_ref\bench\sbom.py`
- `src\anticloud_ref\bench\__init__.py`
- `src\anticloud_ref\crdt\convergence.py`
- `src\anticloud_ref\crdt\gcounter.py`
- `src\anticloud_ref\crdt\lww.py`
- `src\anticloud_ref\crdt\orset.py`
- `src\anticloud_ref\crdt\pncounter.py`
- `src\anticloud_ref\crdt\__init__.py`
- `src\anticloud_ref\deps\lock.py`
- `src\anticloud_ref\deps\__init__.py`
- `src\anticloud_ref\licence\classifier.py`
- `src\anticloud_ref\licence\policy.py`
- `src\anticloud_ref\licence\__init__.py`
- `src\anticloud_ref\perf\harness.py`
- `src\anticloud_ref\perf\__init__.py`
- `src\anticloud_ref\provenance\chain.py`
- `src\anticloud_ref\provenance\__init__.py`
- `src\anticloud_ref\security\safeio.py`
- `src\anticloud_ref\security\secrets.py`
- `src\anticloud_ref\security\validators.py`
- `src\anticloud_ref\security\vault.py`
- `src\anticloud_ref\security\__init__.py`
- `TECHNICAL\01_Architecture.md`
- `TECHNICAL\02_Upstream_Provenance.md`
- `TECHNICAL\03_Verification.md`
- `tests\conftest.py`
- `tests\test_compliance_frameworks.py`
- `tests\test_crdt_convergence.py`
- `tests\test_crdt_gcounter.py`
- `tests\test_crdt_orset.py`
- `tests\test_crdt_pncounter.py`
- `tests\test_licence_policy.py`
- `tests\test_provenance_chain.py`
- `tools\run_bench.py`
- `UPSTREAM\.pre-commit-config.yaml`
- `UPSTREAM\.readthedocs.yml`
- `UPSTREAM\pyproject.toml`
- `UPSTREAM\.github\CONTRIBUTING.md`
- `UPSTREAM\.github\dependabot.yml`
- `UPSTREAM\.github\PULL_REQUEST_TEMPLATE.md`
- `UPSTREAM\.github\workflows\cffconvert.yml`
- `UPSTREAM\.github\workflows\matprep_artifacts.yml`
- `UPSTREAM\.github\workflows\python_build.yml`

**Upstream pin:** `dc018ad5b7d5c37740a58914e269f8996ec6eb6e`
