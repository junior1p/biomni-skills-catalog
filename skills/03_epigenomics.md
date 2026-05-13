<div align="center">

# 🧪 Epigenomics

[![Skills in Category](https://img.shields.io/badge/Skills%20in%20Category-4-4CAF50?style=flat-square)](../README.md)
[![Back to Catalog](https://img.shields.io/badge/Back%20to-Main%20Catalog-blueviolet?style=flat-square)](../README.md)

</div>

---

## Overview

This category covers skills for ChIP-seq, ATAC-seq, DNase-seq, and DNA methylation analysis,
leveraging the ChIP-Atlas public database of 433,000+ experiments.

| # | Skill Name | Skill ID |
|---|---|---|
| 1 | ChIP-Atlas Peak Enrichment | `chip-atlas-peak-enrichment` |
| 2 | ChIP-Atlas Target Genes | `chip-atlas-target-genes` |
| 3 | ChIP-Atlas Diff Analysis | `chip-atlas-diff-analysis` |
| 4 | Upstream Regulator Analysis | `upstream-regulator-analysis` |

---

## 1. ChIP-Atlas Peak Enrichment

- **Skill ID**: `chip-atlas-peak-enrichment`
- **Applicable Scenarios**: TF binding site analysis, histone modification profiling
- **Key Features**:
  - Enrichment analysis against 433,000+ public ChIP-Atlas experiments
  - User-defined genomic region input (BED format)
  - Cross-cell-line and cross-tissue-type comparison
  - Enrichment score calculation and ranking
  - Result visualization and export
- **Data Source**: ChIP-Atlas API (https://chip-atlas.org)

---

## 2. ChIP-Atlas Target Genes

- **Skill ID**: `chip-atlas-target-genes`
- **Applicable Scenarios**: TF target gene prediction, regulatory network construction
- **Key Features**:
  - Pre-computed target gene lists for any transcription factor
  - Filtering by cell line, tissue type, and experiment quality
  - Target gene confidence scoring
  - Integration with differential expression data
  - Functional enrichment of target genes
- **Data Source**: ChIP-Atlas pre-computed database

---

## 3. ChIP-Atlas Diff Analysis

- **Skill ID**: `chip-atlas-diff-analysis`
- **Applicable Scenarios**: Condition-specific epigenetic changes, treatment response
- **Key Features**:
  - Two-group comparison of ChIP-seq / ATAC-seq / DNase-seq experiments
  - Differential peak region (DPR) identification
  - Bisulfite-seq differentially methylated region (DMR) analysis
  - Differential region annotation (genomic location, nearest gene)
  - Differential region visualization and export
- **Data Source**: ChIP-Atlas API

---

## 4. Upstream Regulator Analysis

- **Skill ID**: `upstream-regulator-analysis`
- **Applicable Scenarios**: Transcriptional regulatory mechanism research, drug target discovery
- **Key Features**:
  - Integration of ChIP-Atlas TF binding data with RNA-seq DE results
  - Identification of upstream regulators driving transcriptomic changes
  - TF activity scoring and ranking
  - Regulatory network visualization
  - Cross-condition regulator comparison
- **Dependencies**: ChIP-Atlas API, R/Python

---

<div align="center">

[← Back to Main Catalog](../README.md) &nbsp;|&nbsp; [中文主页](../README_CN.md) &nbsp;|&nbsp; [Contributing](../CONTRIBUTING.md)

*Part of the [Biomni Skills Catalog](https://github.com/junior1p/biomni-skills-catalog) · Maintained by [Phylo](https://phylo.com)*

</div>
