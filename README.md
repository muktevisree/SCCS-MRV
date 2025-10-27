
# Synthetic CCS–MRV Dataset (SCCS-MRV) (v1.3)

[![DOI]https://doi.org/10.5281/zenodo.17330775

## 📘 Overview

This repository hosts the **Synthetic CCS–MRV Dataset (v1.3)** aligned with:

- **OSDU** Well/Facility/Measurement schema entities  
- **Open Footprint (OFP)** models: Facility, Source, Activity, Emission  
- **MRV standards**: EPA 40 CFR Part 98 Subpart RR, ISO 27916, OGMP 2.0  

⚗️ It supports research, ESG reporting, and schema validation using realistic synthetic data across capture, transport, injection, leak simulation, QA, and export stages.

---

## 🧭 OSDU Schema Alignment (2025 Standard)

Aligned with the **OSDU Well-Known Schemas (WKS)** — legacy WKE identifiers are updated to reflect the 2025 standard:

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

## 📂 Repository Structure

```
📦 SCCS-MRV/
├── 📁 schema/                     
│   ├── schema.yaml
│   ├── schema.json
│   └── schema_crosswalk.csv
├── 📁 docs/
│   ├── data_dictionary.csv
│   ├── repo_structure.png
│   └── workflow_diagram.png
├── 📄 ccs_full_dataset_v1.0.csv
├── 📄 ccs_injection_daily_v1.0.csv
├── 📄 ccs_injection_monthly_v1.0.csv
├── 📄 SCCS_MRV_dataset_whitepaper.pdf
├── 📄 example.ipynb
├── 📄 requirements.txt
├── 📄 Dockerfile
├── 📄 LICENSE (CC BY 4.0)
├── 📄 CITATION.cff
├── 📄 README.md
└── 📄 NOTES.md
```

---

## 🔁 Workflow

![Workflow Diagram](docs/workflow_diagram.png)

---

## 📜 License

Distributed under the [Creative Commons Attribution 4.0 License](LICENSE).

---

## 📣 Citation

Please cite this dataset as:

```
Muktevi, Sreekanth (2025). SCCS–MRV Synthetic Dataset v1.3. Zenodo. https://doi.org/10.5281/zenodo.17003094
```

---

## ✨ Acknowledgments

Created as part of the **SynData-ESG Toolkit** to support open-source ESG data generation and validation for net-zero energy systems.

---

## 🧪 Related Projects

- [SGED-OFPOSDU: GHG Dataset](https://zenodo.org/record/17003443)
- [SUHS-OFPOSDU: Hydrogen Storage Dataset](https://zenodo.org/record/17002213)
- [SynData-ESG Toolkit GitHub](https://github.com/muktevisree/SynData-ESG-Toolkit)
