<div align="center">

# 📊 Bulk Omics Analysis

[![Skills in Category](https://img.shields.io/badge/Skills%20in%20Category-6-4CAF50?style=flat-square)](../README.md)
[![Back to Catalog](https://img.shields.io/badge/Back%20to-Main%20Catalog-blueviolet?style=flat-square)](../README.md)

</div>

---

## Overview

This category covers skills for analyzing bulk transcriptomics, proteomics, metabolomics, and multi-omics datasets,
including differential expression, clustering, functional enrichment, and cross-omics integration.

| # | Skill Name | Skill ID |
|---|---|---|
| 1 | Bulk RNA-seq DE (DESeq2) | `bulk-rnaseq-counts-to-de-deseq2` |
| 2 | Bulk Omics Clustering | `bulk-omics-clustering` |
| 3 | Proteomics Diff Exp | `proteomics-diff-exp` |
| 4 | Multi-Omics Integration | `multi-omics-integration` |
| 5 | Functional Enrichment | `functional-enrichment-from-degs` |
| 6 | Co-expression Network | `coexpression-network` |

---

## 1. Bulk RNA-seq DE (DESeq2)

- **Skill ID**: `bulk-rnaseq-counts-to-de-deseq2`
- **Applicable Scenarios**: Bulk RNA-seq differential expression between conditions or groups
- **Key Features**:
  - Raw count matrix input (HTSeq, featureCounts, STAR output)
  - DESeq2 normalization (size factor estimation)
  - Differential expression analysis (Wald test / LRT)
  - Multiple testing correction (Benjamini-Hochberg FDR)
  - Volcano plot, MA plot, and heatmap visualization
  - Ranked gene list output for downstream GSEA
- **Dependencies**: DESeq2, ggplot2, R/Bioconductor

---

## 2. Bulk Omics Clustering

- **Skill ID**: `bulk-omics-clustering`
- **Applicable Scenarios**: Sample grouping, subtype discovery, batch effect assessment
- **Key Features**:
  - Hierarchical clustering (Ward, complete linkage)
  - k-means / PAM clustering with optimal k selection
  - PCA / UMAP dimensionality reduction and visualization
  - Heatmap with annotation tracks (ComplexHeatmap)
  - Sample correlation matrix
  - Batch effect evaluation and visualization
- **Dependencies**: ComplexHeatmap, factoextra, umap, R

---

## 3. Proteomics Diff Exp

- **Skill ID**: `proteomics-diff-exp`
- **Applicable Scenarios**: Mass spectrometry proteomics differential protein analysis
- **Key Features**:
  - MaxQuant / Proteome Discoverer output processing
  - PSM-aware variance estimation (DEqMS)
  - limma linear model differential analysis
  - Missing value handling (MinProb / KNN imputation)
  - Protein abundance normalization (median, quantile)
  - Volcano plot and result table export
- **Dependencies**: limma, DEqMS, R/Bioconductor

---

## 4. Multi-Omics Integration

- **Skill ID**: `multi-omics-integration`
- **Applicable Scenarios**: Multi-omics joint analysis, biomarker discovery, patient stratification
- **Key Features**:
  - Supports transcriptomics + proteomics + metabolomics and more
  - MOFA+ latent factor decomposition
  - Cross-omics variance decomposition per factor
  - Factor biological interpretation (enrichment, correlation)
  - Sample stratification and subtype discovery
- **Dependencies**: MOFA+, mofapy2, Python/R

---

## 5. Functional Enrichment

- **Skill ID**: `functional-enrichment-from-degs`
- **Applicable Scenarios**: Differential gene functional interpretation, pathway analysis
- **Key Features**:
  - Over-representation analysis (ORA): GO, KEGG, Reactome, WikiPathways
  - Gene Set Enrichment Analysis (GSEA) with ranked gene lists
  - MSigDB gene set support (Hallmarks, C2, C5, etc.)
  - Enrichment result visualization (dot plot, bar plot, network plot, GSEA plot)
  - Multi-condition enrichment comparison
- **Dependencies**: clusterProfiler, enrichplot, msigdbr, R

---

## 6. Co-expression Network

- **Skill ID**: `coexpression-network`
- **Applicable Scenarios**: Gene functional module discovery, hub gene identification, trait correlation
- **Key Features**:
  - WGCNA weighted co-expression network construction
  - Soft-thresholding power selection
  - Module identification and eigengene extraction
  - Module-trait correlation analysis
  - Hub gene (intramodular connectivity) identification
  - Cytoscape-compatible network export
- **Dependencies**: WGCNA, R

---

<div align="center">

[← Back to Main Catalog](../README.md) &nbsp;|&nbsp; [中文主页](../README_CN.md) &nbsp;|&nbsp; [Contributing](../CONTRIBUTING.md)

*Part of the [Biomni Skills Catalog](https://github.com/junior1p/biomni-skills-catalog) · Maintained by [Phylo](https://phylo.com)*

</div>
