# Synthetic CCS–MRV Dataset (SCCS-MRV) (v1.0)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17003094.svg)](https://doi.org/10.5281/zenodo.17003094)

## Overview
This repository hosts the **Synthetic CCS–MRV Dataset (v1.0)** aligned with:
- **OSDU** Well/Wellbore/Facility entities
- **Open Footprint (OFP)** model (Facility, Source, Activity, Measurement, Emission)
- **MRV standards**: EPA 40 CFR Part 98 Subpart RR, ISO 27916, OGMP 2.0

The dataset provides synthetic but realistic CCS records (annual, monthly, daily) for research, standards testing, and ESG reporting.

## Repository Contents
- `data/ccs_full_dataset_v1.0.csv` – Facility-level annual summary
- `data/ccs_injection_daily_v1.0.csv` – Daily injection timeseries
- `data/ccs_injection_monthly_v1.0.csv` – Monthly roll-up
- `schema/schema.yaml` – Dataset schema
- `schema/schema_crosswalk.csv` – Field mappings (OSDU, OFP, MRV)
- `docs/NOTES.md` – Methodology and QA notes
- `docs/SCCS_MRV_dataset_whitepaper.pdf` – White paper (design, validation, use cases)
- `LICENSE.txt` – License (CC BY 4.0)
- `CITATION.cff` – Citation metadata

## Usage
Clone the repo and install dependencies:
```bash
pip install -r requirements.txt
```

Load dataset in Python:
```python
import pandas as pd
df = pd.read_csv("data/ccs_injection_daily_v1.0.csv")
print(df.head())
```

## Authors
- **Sreekanth Muktevi** – Lead & Corresponding Author
- **Yogesh Nagpal** – Sustainability domain expertise
- **Rajesh Leela Thotakura** – Data engineering, schema, QA scripts
- **Jyotsna Muktevi** – Documentation, workflow alignment

## License
Creative Commons Attribution 4.0 (CC-BY 4.0).

## Citation
Muktevi, S., Nagpal, Y., Thotakura, R. L., & Muktevi, J. (2025). *SCCS–MRV Synthetic Dataset (v1.0)* [Data set]. Zenodo. https://doi.org/10.5281/zenodo.17003094

## Disclaimer
This dataset is **fully synthetic**. It does not represent any real CCS facility or reservoir data. Provided only for research, teaching, and prototyping.
