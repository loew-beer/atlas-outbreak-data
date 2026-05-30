# Atlas Outbreak Data

Open data, methodology, and source documentation from the Atlas Outbreak Intelligence platform.

## Current: Ebola DRC 2026 (BDBV)

Bundibugyo ebolavirus outbreak in the Democratic Republic of the Congo and Uganda. PHEIC declared 2026-05-17.

### Live Dashboard

**[outbreak.loew-beer.at](https://outbreak.loew-beer.at)** -- interactive 10-tab outbreak intelligence dashboard with maps, epi curve, genomic context, and response tracking.

### Available Data

| File | Description | Licence |
|---|---|---|
| [data_provenance.csv](ebola-drc-2026/data_provenance.csv) | 9 data sources with access dates, record counts, and use terms | CC-BY-4.0 |
| [sequence_metadata.csv](ebola-drc-2026/sequence_metadata.csv) | BDBV sequence accession metadata (GenBank public domain entries) | CC-BY-4.0 |
| [phylo_analysis.md](ebola-drc-2026/phylo_analysis.md) | Phylogenetic analysis report with data source hierarchy | CC-BY-4.0 |
| [bdbv_dataset_qc_improved.png](ebola-drc-2026/bdbv_dataset_qc_improved.png) | QC figure: historical genome dataset assessment (300 DPI) | CC-BY-4.0 |
| [figure_caption.txt](ebola-drc-2026/figure_caption.txt) | Methodological caption for QC figure | CC-BY-4.0 |

### Methodology

See [METHODOLOGY.md](METHODOLOGY.md) for data collection, processing, and epistemic standards.

### Data Sources

Full source list with 43 URLs and access dates: [DATA_SOURCES.md](ebola-drc-2026/DATA_SOURCES.md)

**Primary epidemiological:** INSP SitRep via INRB-UMIE, WHO DON602/603, ECDC Threat Assessment Brief
**Primary genomic:** Pathoplexus (Restricted Use), Virological.org, Nextstrain, NCBI GenBank
**Secondary:** Reuters/WHO briefing, The Lancet, MSF

### What Is Not in This Repo

- The interactive dashboard (served at [outbreak.loew-beer.at](https://outbreak.loew-beer.at))
- INSP SitRep extracted data (cite INRB-UMIE directly: [github.com/INRB-UMIE/Ebola_DRC_2026](https://github.com/INRB-UMIE/Ebola_DRC_2026))
- Pathoplexus genome sequences (Restricted Use licence; access via [pathoplexus.org](https://pathoplexus.org/ebola-bdbv/search))
- Individual-level patient data (none exists in this project; all analysis from aggregate reports)

## Licence

Content and analysis: CC-BY-4.0. Third-party data retains original licences (see data_provenance.csv).

## Citation

Atlas Outbreak Intelligence. Ebola DRC 2026: Bundibugyo Ebolavirus Open Data and Methodology. https://github.com/loew-beer/atlas-outbreak-data

## Contact

- Email: [office@loew-beer.at](mailto:office@loew-beer.at)
- Dashboard: [outbreak.loew-beer.at](https://outbreak.loew-beer.at)
- Telegram: coming soon
