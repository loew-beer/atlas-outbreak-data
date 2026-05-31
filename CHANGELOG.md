# Changelog

## v5 -- 2026-05-31

- Health-zone stacked epi curve: daily confirmed cases broken down by top 6 zones (Bunia, Rwampara, Mongbalu, Nyakunde, Katwa, Butembo). Added to dashboard C. Time tab and PDF situation report.
- Collection-to-release sequencing turnaround: median 15 days (range 4-18) from sample collection to Pathoplexus release. Added to dashboard G. Genomics tab and PDF.
- Province choropleth: PDF maps now shade health zones by province (Ituri, Nord-Kivu, Sud-Kivu) with distinct colours and province legend.
- Death count corrected to CDC 2026-05-29 figures: 19 confirmed deaths (17 DRC + 2 Uganda), 223 suspected, 242 total.
- Cross-validation pipeline: automated pre-publish check runs before every sync and every daily briefing. Flags discrepancies between INSP, WHO, CDC.
- Data access requirements document: specifies exactly what data, system, and contact is needed to unlock each dormant dashboard module.
- Ingestion pipeline: drop-in CSV processing for linelist, contacts, lab results, genomic linkage.
- Epi curve CSS fix: missing class definitions added to dashboard stylesheet.
- JSON fetch 404 fix: absolute path for VPS serving context.

## v4 -- 2026-05-30

- INRB-UMIE data integration: daily INSP SitRep data (21 health zones, 12 reporting days)
- Attack rates computed with WorldPop denominators (Rwampara 425.8/100k highest)
- PCR capacity mapped: 36 machines across 19 zones
- Contact tracing cascade: 2,417 cumulative contacts traced
- Real epi curve by notification date
- All three geographic maps rebuilt with INRB-UMIE data and real health zone centroids
- Dashboard rebuilt with subnational operational data across all 10 tabs

## v3 -- 2026-05-30

- Peer review corrections applied
- CFR relabelled as raw death proportions; WHO 30-50% estimate added
- "Zoonotic introduction" softened to "separate introduction relative to sampled historical lineages"
- Goma claims marked as unverified (requires DRC MOH/WHO subnational data)
- Uganda source attribution corrected (Reuters/WHO briefing, not DON602)
- Three-tier source hierarchy (primary epi, primary genomic, secondary/media)
- Province figures marked as working estimates
- Executive summary added
- Presentation package documented
- Source-lock verified

## v2 -- 2026-05-30

- Pathoplexus 2026 sequences identified (16 outbreak genomes, May 2026)
- Data sources updated from 38 to 43
- Genomic data gap reclassified from "critical" to "partially addressed, update required"
- 10-tab outbreak control dashboard built (WHO Outbreak Toolkit standard)
- Atlas/HELIOS branding applied
- Self-contained HTML (no CDN dependencies except Leaflet for maps)
- QC figure improved with scientific rigour corrections

## v1 -- 2026-05-29

- Initial evidence scan
- 38 sources catalogued
- Genomic section reported 0 current outbreak sequences
- 4-tab dashboard prototype
- Phylogenetic analysis: 34 historical NCBI GenBank sequences
