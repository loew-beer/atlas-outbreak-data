# Methodology

## Classification

This is an **evidence scan**, not a systematic review. It does not follow PRISMA methodology and does not claim exhaustive literature coverage.

## Data Collection

### Epidemiological Data
- Primary source: INSP SitRep MVE 001-012 via INRB-UMIE GitHub repository
- Daily notification-date case counts by health zone (21 zones, 12 reporting days)
- Contact tracing cumulative totals, hospitalisation data
- INSP data manually transcribed from PDF situation reports; transcription errors possible
- Supplemented by WHO Disease Outbreak News (DON602, DON603, DON605) for national-level figures
- Uganda data from Uganda MOH via Reuters/WHO briefing

### Population Denominators
- WorldPop gridded population estimates aggregated to DRC health zone level
- Source: INRB-UMIE repository (GRID3/WorldPop methodology)
- Attack rates computed as: (total reported cases / WorldPop population) x 100,000

### Testing Capacity
- PCR machine counts per health zone from INRB-UMIE testing_capacity dataset
- Static snapshot; does not reflect throughput, staffing, or reagent availability

### Genomic Data
- Historical sequences (34): NCBI GenBank (public domain)
- Current outbreak sequences (16): Pathoplexus (Restricted Use licence)
- Phylogenetic context: Virological.org rapid communication (Amuri-Aziza et al., 2026)
- Cross-validation: Nextstrain ebola/bdbv interactive phylogeny
- Local analysis uses historical genomes only; Pathoplexus 2026 sequences identified but not yet incorporated

### Geographic Data
- Health zone boundaries: DRC Ministry of Health via INRB-UMIE shapefile (519 zones)
- Centroids computed from polygon geometry
- Border distances approximate (centroid to nearest border point)

## Processing

- Data extracted from INRB-UMIE processed CSVs using Python standard library
- Attack rates, confirmation rates, and contact-to-case ratios calculated from source data
- QC figure generated using matplotlib (Python)
- Dashboard is self-contained HTML/CSS/JS with no external computational dependencies
- Geographic maps use Leaflet.js with OpenStreetMap tiles

## Limitations

1. Notification date, not onset date - true epi curve shape unknown
2. Province-level case allocations are working estimates, not official MOH figures
3. INSP data manually transcribed from PDF - possible transcription errors
4. WorldPop denominators are modelled estimates, not census data
5. Conflict-driven displacement makes population denominators unreliable
6. Genomic coverage biased toward Ituri and early May 2026
7. Contact tracing follow-up rates mostly not declared in INSP data
8. Goma-specific case status requires verification from subnational WHO/MOH data

## Epistemic Standards

- Every epidemiological number has a source and date
- CFR presented as raw death proportions with right-censoring caveat, not finalised rates
- Phylogenetic claims limited to "separate introduction relative to sampled historical lineages"
- Province figures labelled as working estimates
- Data gaps explicitly documented in each section
- Source counts identified as snapshot-dependent
