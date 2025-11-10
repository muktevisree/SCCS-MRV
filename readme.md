# Synthetic CCS–MRV Dataset (SCCS-MRV) (v1.5)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17003094.svg)](https://doi.org/10.5281/zenodo.17003094)

## 📘 Overview

This repository hosts the **Synthetic CCS–MRV Dataset (v1.5)**, a comprehensive and openly accessible dataset built to support carbon capture and storage (CCS) MRV (Monitoring, Reporting, Verification) workflows. It is aligned with:

- **Open Footprint (OFP v1.0.2)** emissions and mass-balance model  
- **Open Subsurface Data Universe (OSDU v3.0.1)** WKS entities: Facility, Wellbore, Measurement, etc.  
- **CCS MRV standards** including EPA 40 CFR Part 98 Subpart RR, ISO 27916, and OGMP 2.0

💡 The dataset enables benchmarking, tool development, schema validation, synthetic modeling, and academic training related to CCS.

---

## 🧭 OSDU Schema Alignment

Updated to the 2025 schema standards:

| Group                  | Entity             | WKS ID                                         |
|------------------------|--------------------|------------------------------------------------|
| Master Data            | Facility           | `WKS:master-data--Facility:1.0.0`              |
| Master Data            | Asset              | `WKS:master-data--Asset:1.0.0`                 |
| Master Data            | Wellbore           | `WKS:master-data--Wellbore:1.0.0`              |
| Work Product Component | Measurement        | `WKS:work-product-component--Measurement:1.0.0`|
| Work Product Component | ProductionData     | `WKS:work-product-component--ProductionData:1.0.0` |
| Work Product Component | EventMethod        | `WKS:work-product-component--EventMethod:1.0.0`|
| Extension (Proposed)   | EnvironmentalData  | `WKS:extension--EnvironmentalData:1.0.0`       |

---

## 📦 Repository Structure
📦 SCCS-MRV/
├── 📁 schema/
│   ├── schema.yaml                     # Unified data dictionary
│   ├── schema.json                     # JSON schema for validation
│   └── schema_crosswalk.csv           # Field mapping to OFP/OSDU standards
├── 📁 docs/
│   ├── data_dictionary.csv
│   ├── repo_structure.png             # Figure 2 – Repository layout
│   ├── workflow_diagram.png           # Figure 3 – Data aggregation logic
│   └── example_payload.json           # Sample OFP–OSDU JSON payload
├── 📄 ccs_full_dataset_v1.0.csv
├── 📄 ccs_injection_daily_v1.0.csv
├── 📄 ccs_injection_monthly_v1.0.csv
├── 📄 SCCS_MRV_dataset_whitepaper.pdf
├── 📄 example.ipynb                   # Jupyter notebook: regeneration & validation
├── 📄 requirements.txt
├── 📄 Dockerfile
├── 📄 LICENSE                         # CC-BY 4.0 License
├── 📄 CITATION.cff
├── 📄 README.md
└── 📄 NOTES.md

---

## 🔁 Workflow

![Workflow Diagram](docs/workflow_diagram.png)

Synthetic records simulate CO₂ capture, transport, injection, and monitoring across 10 facilities using deterministic logic and schema-aligned formats. Reuse scenarios include:

- Digital twin simulation
- ESG platform testing
- Schema validator development
- Academic education

---

## 📊 Record Summary

| File                         | Records × Fields  | Notes                                 |
|-----------------------------|-------------------|----------------------------------------|
| ccs_full_dataset_v1.0.csv   | 10 × 26           | Facility-level annual summaries        |
| ccs_injection_daily_v1.0.csv| 3,660 × 4         | Daily injection and monitoring         |
| ccs_injection_monthly_v1.0.csv | 120 × 3        | Monthly aggregations with leak data   |

---

## ⚙️ Reproducibility

- ✅ Fixed random seed (42) for deterministic generation  
- ✅ Unified schema and codebook (`schema.yaml`)  
- ✅ Validation logs, checksum report (`integrity_report.txt`)  
- ✅ Dockerfile for containerized execution  
- ✅ Machine-readable metadata (`ccs_dataset-metadata.yaml`)  
- ✅ Jupyter notebook includes regeneration, validation, and schema-aligned OFP/OSDU export examples

---

## 📜 License

Distributed under the [Creative Commons Attribution 4.0 License](LICENSE).

---

## 📣 Citation

Please cite this dataset as:

```bibtex
@dataset{muktevi_sccs_mrv_2025,
  author       = {Sreekanth Muktevi and Yogesh Nagpal and Rajesh Leela Thotakura and Jyotsna Muktevi},
  title        = {SCCS–MRV Synthetic Dataset (v1.5)},
  year         = 2025,
  doi          = {10.5281/zenodo.17003094},
  publisher    = {Zenodo},
  url          = {https://doi.org/10.5281/zenodo.17003094}
}

🧪 Related Projects
	•	SGED-OFPOSDU: Synthetic GHG Dataset￼
	•	SUHS-OFPOSDU: Underground Hydrogen Storage￼
	•	SynData-ESG Toolkit (GitHub)￼

---

🙌 Acknowledgments

This dataset was developed as part of the SynData-ESG Toolkit initiative. It supports ESG disclosure innovation, schema interoperability, and digital net-zero platform enablement.
