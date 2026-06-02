# Atlas Outbreak Data

Open data and methodology from the Atlas Outbreak Intelligence platform.

## Current: Ebola DRC 2026 (BDBV)

Bundibugyo ebolavirus outbreak in the Democratic Republic of the Congo and Uganda. PHEIC declared 2026-05-17.

**Live dashboard:** [outbreak.loew-beer.at](https://outbreak.loew-beer.at)

---

### Structured Data

Zone-level epidemiological data extracted from INSP SitReps via [INRB-UMIE](https://github.com/INRB-UMIE/Ebola_DRC_2026) (MIT licence). Snapshot covers 2026-05-14 to 2026-05-30, 23 affected health zones.

| File | Description |
|---|---|
| [data/inrb_umie_data.json](ebola-drc-2026/data/inrb_umie_data.json) | Full zone-level dataset: epi curve, cumulative national, cases by zone, attack rates, contact tracing, PCR capacity |
| [data/outbreak_summary.json](ebola-drc-2026/data/outbreak_summary.json) | Headline figures from CDC, WHO, and ECDC (confirmed cases, deaths, geographic spread) |
| [data/epi_curve_by_zone.json](ebola-drc-2026/data/epi_curve_by_zone.json) | Daily confirmed cases per health zone (JSON array) |
| [data/epi_curve_daily.csv](ebola-drc-2026/data/epi_curve_daily.csv) | National daily confirmed and suspected cases |
| [data/cumulative_national.csv](ebola-drc-2026/data/cumulative_national.csv) | Cumulative national case and death counts by date |
| [data/cases_by_zone.csv](ebola-drc-2026/data/cases_by_zone.csv) | Total confirmed and suspected cases by health zone |
| [data/contact_tracing.csv](ebola-drc-2026/data/contact_tracing.csv) | Contact tracing cascade by date |
| [data/pcr_capacity.csv](ebola-drc-2026/data/pcr_capacity.csv) | PCR machines per health zone |

Data files are updated on each sync (every ~3 hours). All figures carry uncertainty; see `data_provenance.csv` and `DATA_SOURCES.md` for source details and snapshot dates.

---

### Daily Situation Reports

PDF briefings and machine-readable CSV packages, generated daily at 07:00 UTC.

| Date | PDF | CSV package |
|---|---|---|
| 2026-06-02 | [2026-06-02.pdf](ebola-drc-2026/briefings/2026-06-02.pdf) | [briefings/2026-06-02/](ebola-drc-2026/briefings/2026-06-02/) |
| 2026-06-01 | [2026-06-01.pdf](ebola-drc-2026/briefings/2026-06-01.pdf) | [briefings/2026-06-01/](ebola-drc-2026/briefings/2026-06-01/) |
| 2026-05-31 | [2026-05-31.pdf](ebola-drc-2026/briefings/2026-05-31.pdf) | [briefings/2026-05-31/](ebola-drc-2026/briefings/2026-05-31/) |
| 2026-05-30 | [2026-05-30.pdf](ebola-drc-2026/briefings/2026-05-30.pdf) | [briefings/2026-05-30/](ebola-drc-2026/briefings/2026-05-30/) |

See [briefings/DISCLAIMER.txt](ebola-drc-2026/briefings/DISCLAIMER.txt) before use.

---

### Genomic Analysis

| File | Description | Licence |
|---|---|---|
| [sequence_metadata.csv](ebola-drc-2026/sequence_metadata.csv) | BDBV accession metadata (NCBI GenBank, public domain) | CC-BY-4.0 |
| [data_provenance.csv](ebola-drc-2026/data_provenance.csv) | 9 data sources with access dates, record counts, and use terms | CC-BY-4.0 |
| [phylo_analysis.md](ebola-drc-2026/phylo_analysis.md) | Phylogenetic analysis report | CC-BY-4.0 |
| [bdbv_dataset_qc_improved.png](ebola-drc-2026/bdbv_dataset_qc_improved.png) | QC figure: historical genome dataset (300 DPI) | CC-BY-4.0 |

---

### Methodology and Sources

- [METHODOLOGY.md](METHODOLOGY.md) — data collection, processing, and epistemic standards
- [CHANGELOG.md](CHANGELOG.md) — version history and corrections
- [DATA_SOURCES.md](ebola-drc-2026/DATA_SOURCES.md) — full source list with URLs and access dates

---

### What Is Not in This Repo

- Pathoplexus genome sequences — Restricted Use licence; access via [pathoplexus.org](https://pathoplexus.org/ebola-bdbv/search)
- Individual-level patient data — none exists in this project; all analysis is from aggregate public reports
- Interactive dashboard source — served at [outbreak.loew-beer.at](https://outbreak.loew-beer.at)

---

## Disclaimer

This is an independent secondary-surveillance repository; not an official outbreak report. Data and visualizations are generated from public/cited sources and may differ from official reports. Interpret with caution and verify primary sources before use in clinical, operational, or policy decisions.

## Licence

Content and analysis: CC-BY-4.0. Third-party data retains original licences (see [data_provenance.csv](ebola-drc-2026/data_provenance.csv)).

## Citation

Atlas Outbreak Intelligence. Ebola DRC 2026: Open Data and Situation Reports. https://github.com/loew-beer/atlas-outbreak-data

## Contact

- Email: [office@loew-beer.at](mailto:office@loew-beer.at)
- Dashboard: [outbreak.loew-beer.at](https://outbreak.loew-beer.at)
