# BDBV Phylogenetic Analysis -- DRC Outbreak 2024-2026

## Genomic Analysis Report -- atlas-bioinformatician
**Sample(s):** 34 BDBV isolates (local analysis); 60 total available on Pathoplexus (as of 2026-05-30)
**Analysis type:** Sequence analysis and phylogenetic characterization
**Tools used:** Biopython, matplotlib, genetic distance calculations
**Analysis date:** 2026-05-29 (initial); 2026-05-30 (data source update)

## Analysis Status

**The local analysis currently uses 34 historical NCBI GenBank sequences only.**
Initial 2026 outbreak genomes are now available via Pathoplexus and should be incorporated.
The figure and statistics below reflect the historical-only dataset until the pipeline is rerun with Pathoplexus data.

## Data Sources

### Primary Genomic Sources

| Source | Type | Records | Status in Local Analysis |
|--------|------|---------|--------------------------|
| **Pathoplexus** | Primary 2026 outbreak genomes | 16 sequences (May 2026) | NOT YET INCORPORATED |
| **NCBI GenBank** | Historical reference genomes | 34 sequences (2007, 2012) | Incorporated |
| **Virological.org** | Rapid communication describing initial genomes | 13+ genomes described | Used for context only |
| **Nextstrain** | Visualization and cross-check | Combined historical + 2026 tree | Used for validation only |

### Epidemiological Sources

| Source | Type | Use |
|--------|------|-----|
| **WHO** | Primary epidemiological | DON602, DON603, PHEIC declaration 2026-05-17, situation reports |
| **ECDC** | Secondary risk assessment | EU/EEA threat assessment brief, uncertainty language |
| **CDC** | Situational awareness | HAN 00530 |
| **Reuters/AP** | Rapid updates only | Date-stamped; does not override WHO figures |

### Data Not Used

| Source | Reason |
|--------|--------|
| **GISAID** | No confirmed BDBV records found; not a primary BDBV source |

## Available 2026 Outbreak Genomes (Pathoplexus)

As of 2026-05-30, 16 sequences from the current outbreak are publicly accessible on Pathoplexus under the "Restricted" licence (public health use; contact before publication):

| Accession | Country | Admin Level 1 | Location | Collection Date |
|-----------|---------|---------------|----------|-----------------|
| PP_006XHL9.1 | DRC | Ituri | Bunia | 2026-05-03 |
| PP_006XHKB.1 | DRC | Ituri | Bunia | 2026-05 |
| PP_006XCJJ.1 | Uganda | Kampala | Kampala | 2026-05-14 |
| PP_006XXY5.1 | Germany | -- | imported case | 2026-05 |
| PP_006Y8NC.1 | DRC | North-Kivu | Katwa | 2026-05-06 |
| PP_006Y8PA.1 | DRC | Ituri | Hoho | 2026-05-03 |
| PP_006Y8Q8.1 | DRC | Ituri | Lumumba | 2026-05-03 |
| PP_006Y8R6.1 | DRC | Ituri | -- | 2026-05 |
| PP_006Y8S4.1 | DRC | Ituri | -- | 2026-05 |
| PP_00711R7.1 | DRC | Ituri | -- | 2026-05 |
| PP_00711S5.1 | DRC | Ituri | -- | 2026-05 |
| PP_00711T3.1 | DRC | Ituri | -- | 2026-05 |
| PP_00711U1.1 | DRC | Ituri | -- | 2026-05 |
| PP_00711VZ.1 | DRC | Ituri | -- | 2026-05 |
| PP_00712Q8.1 | DRC | Ituri | -- | 2026-05 |

Authors: Amuri-Aziza, Quick, Loman, Rambaut (INRB); Dept. National Health Laboratory (Uganda).

**Data use terms:** Pathoplexus "Restricted" licence. Contact lead investigators (Prof. Placide Mbala-Kingebeni, INRB; Dr. Isaac Ssewanyana, CPHL Uganda) before publication use.

## Sequencing Workflow (from Virological.org Rapid Communication)

- **RNA extraction:** QIAGEN viral RNA kit
- **Library preparation:** Illumina RNA Prep with Enrichment + Twist Comprehensive Viral Research panel
- **Sequencing platforms:** Nextseq1000/2000, GridION
- **Bioinformatics:** czid, nf-core/viralrecon v3.0.0, Nextflow v25.10.2
- **Phylogenetic pipeline:** RACCOON (MAFFT alignment + IQ-TREE2 maximum-likelihood, HKY+gamma model)
- **Historical context:** 34 BDBV genomes from 2007 Uganda and 2012 DRC outbreaks

## Local Analysis Results (Historical Genomes Only)

### Sequence Dataset Composition
- **Total sequences in local analysis:** 34
- **Sequence length range:** 18,277 -- 18,942 bp
- **Mean sequence length:** 18,601 bp
- **Source database:** NCBI GenBank

### Geographic Distribution (Local Dataset)
- **DRC-Isiro (2012):** 19 sequences (55.9%)
- **Uganda-Bundibugyo (2007):** 15 sequences (44.1%)

Note: The "Unknown" category from the initial analysis has been reclassified based on accession metadata. Some sequences listed as "Unknown" country in GenBank are attributable to Uganda 2007 or DRC 2012 based on strain names and publication context.

### Temporal Distribution (Local Dataset)
- **Sequences with dates:** 33/34
- **2007:** 10 sequences
- **2012:** 23 sequences
- **2024--2026:** 0 sequences (available on Pathoplexus but not yet incorporated)

### Genetic Diversity Analysis (Local Dataset)
- **Mean genetic distance:** 0.2630
- **Distance range:** 0.000 -- 0.788
- **Pairwise comparisons analyzed:** 40

**Methodological caveat:** The distance metric used in the local analysis has not been verified against the RACCOON pipeline output. Verify alignment quality, gap/N handling, and distance metric before biological interpretation. The mean distance of 0.2630 likely reflects inter-outbreak divergence (2007 vs 2012) rather than within-outbreak diversity.

### Reference Genomes in Dataset

| Accession | Description | Year | Country | Notes |
|-----------|-------------|------|---------|-------|
| NC_014373.1 | BDBV RefSeq reference | 2007 | Uganda | RefSeq standard |
| FJ217161.1 | BDBV complete genome | 2007 | Uganda | Original 2007 isolate |
| KC545393.1 | EboBund-112 | 2012 | DRC | Complete DRC 2012 genome |
| KC545394.1 | EboBund-120 | 2012 | DRC | Complete DRC 2012 genome |
| KC545395.1 | EboBund-122 | 2012 | DRC | Complete DRC 2012 genome |
| KC545396.1 | EboBund-14 | 2012 | DRC | Complete DRC 2012 genome |

## Preliminary Findings from External Sources (Virological.org / Nextstrain)

The RACCOON pipeline analysis reported in Virological.org (Amuri-Aziza et al., May 2026) provides the following preliminary findings from the 2026 outbreak genomes:

1. **tMRCA estimate:** Late February to late April 2026 (depending on evolutionary rate assumptions)
2. **ADAR editing:** Evidence of host ADAR editing in one genome (4 T-to-C mutations)
3. **Outbreak classification:** Third documented Bundibugyo outbreak; second caused by BDBV species
4. **Phylogenetic placement:** 2026 genomes form a distinct clade relative to sampled 2007 and 2012 lineages (per Nextstrain visualisation). This is consistent with a separate introduction; zoonotic origin is plausible for Ebola virus disease but cannot be directly demonstrated from human genome data alone.

**These findings are from external analyses and have not been reproduced locally.**

**Sequence count note:** Counts differ by source because each represents a different snapshot, access level, QC filter, and curation scope. Pathoplexus is the primary repository (~54-60 records visible depending on filters and access); Nextstrain displays a curated subset (~45); the local Atlas analysis contains only the 34 historical NCBI GenBank sequences. These are overlapping subsets, not additive totals.

## Transmission Inference Limitation

Current genomes are sufficient for preliminary phylogenetic placement, but not for robust transmission-chain inference unless broader sampling, dates, metadata, and epidemiological links are available.

Even with initial 2026 genomes incorporated, the following limitations apply:
- 16 genomes from a multi-hundred-case outbreak represents less than 15% genomic coverage
- Collection dates cluster in early May 2026; later transmission phases are unsampled
- Sub-health-zone geographic resolution is incomplete
- No linked epidemiological data (contact tracing, onset dates, exposure history)

## Major Limitations and Data Gaps

1. **Local analysis uses historical genomes only** -- 2026 Pathoplexus genomes identified but not yet incorporated
2. **Limited 2026 genomic coverage** -- 16 genomes from hundreds of confirmed cases
3. **Temporal sampling bias** -- all 2026 genomes from early May; no late May or ongoing transmission data
4. **Geographic metadata gaps** -- many 2026 sequences lack sub-provincial location detail
5. **Restricted data licence** -- Pathoplexus "Restricted" terms require contact before publication
6. **No linked epi-genomic data** -- sequences lack case-level epidemiological metadata
7. **Distance metric unverified** -- local analysis distance calculations need validation against RACCOON pipeline

## Recommended Next Steps

### Immediate (Priority 1)
1. Download 2026 Pathoplexus sequences and incorporate into local analysis
2. Rerun alignment (MAFFT) and phylogenetic reconstruction (IQ-TREE2, HKY+gamma) to match RACCOON pipeline
3. Cross-validate local tree topology against Nextstrain ebola/bdbv

### Short-term (Priority 2)
4. Contact lead investigators (Mbala-Kingebeni, Ssewanyana) for publication terms and additional metadata
5. Map 2026 sequences to health zones for geographic risk assessment
6. Estimate within-outbreak diversity for 2026 clade

### Medium-term (Priority 3)
7. Temporal phylogenetics (BEAST2) when sufficient longitudinal sampling available
8. Geographic phylogenetics (spatial diffusion) when sub-provincial metadata available
9. Integrate with epidemiological contact tracing data for transmission reconstruction

## Figure Labels

The current local analysis figure should be labelled:
**"Historical-genome analysis only -- update required with available 2026 Pathoplexus genomes"**

Once 2026 genomes are incorporated, the figure should be relabelled:
**"BDBV genomic context including initial May 2026 outbreak genomes"**

---
*Report generated by Atlas Bioinformatician on 2026-05-29; data source update 2026-05-30*
*See data_provenance.csv and sequence_metadata.csv for full source documentation*
