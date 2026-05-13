<div align="center">

# 🔬 Single-Cell & Spatial Transcriptomics

[![Skills in Category](https://img.shields.io/badge/Skills%20in%20Category-7-4CAF50?style=flat-square)](../README.md)
[![Back to Catalog](https://img.shields.io/badge/Back%20to-Main%20Catalog-blueviolet?style=flat-square)](../README.md)

</div>

---

## Overview

This category covers skills for analyzing single-cell RNA sequencing (scRNA-seq) and spatial transcriptomics data,
from raw count matrices through cell type annotation, trajectory inference, cell communication, and regulatory network analysis.

| # | Skill Name | Skill ID |
|---|---|---|
| 1 | scRNAseq Scanpy Core Analysis | `scrnaseq-scanpy-core-analysis` |
| 2 | scRNAseq Seurat Core Analysis | `scrnaseq-seurat-core-analysis` |
| 3 | scRNA Trajectory Inference | `scrna-trajectory-inference` |
| 4 | Cell-Cell Communication | `cell-cell-communication` |
| 5 | GRN pySCENIC | `grn-pyscenic` |
| 6 | Spatial Transcriptomics | `spatial-transcriptomics` |
| 7 | Pooled CRISPR Screens | `pooled-crispr-screens` |

---

## 1. scRNAseq Scanpy Core Analysis

- **Skill ID**: `scrnaseq-scanpy-core-analysis`
- **Applicable Scenarios**: 10x Genomics, Smart-seq2, and other scRNA-seq platforms
- **Key Features**:
  - Quality control: filtering low-quality cells and genes (mitochondrial %, doublet detection)
  - Normalization, log-transformation, and highly variable gene selection
  - PCA dimensionality reduction, neighborhood graph construction
  - UMAP / t-SNE visualization
  - Leiden / Louvain clustering
  - Differential expression gene identification per cluster
  - Automated cell type annotation
- **Dependencies**: Scanpy, AnnData, scvi-tools, Python

---

## 2. scRNAseq Seurat Core Analysis

- **Skill ID**: `scrnaseq-seurat-core-analysis`
- **Applicable Scenarios**: 10x Genomics, Drop-seq, and other droplet-based platforms
- **Key Features**:
  - Quality control and cell filtering
  - SCTransform normalization (variance-stabilizing)
  - PCA, UMAP dimensionality reduction and visualization
  - Graph-based clustering (FindClusters)
  - Differential expression analysis (FindMarkers, Wilcoxon / MAST)
  - Cell type annotation with marker genes
  - Multi-sample integration (Harmony / CCA / RPCA)
- **Dependencies**: Seurat v5, R/Bioconductor

---

## 3. scRNA Trajectory Inference

- **Skill ID**: `scrna-trajectory-inference`
- **Applicable Scenarios**: Developmental biology, cell differentiation, stem cell research
- **Key Features**:
  - Pseudotime ordering along differentiation trajectories
  - Trajectory inference using Monocle3 / PAGA
  - RNA velocity analysis (scVelo) for directional dynamics
  - Cell fate probability estimation (CellRank)
  - Trajectory-associated differential gene expression
- **Dependencies**: Monocle3, scVelo, CellRank, PAGA, Python/R

---

## 4. Cell-Cell Communication

- **Skill ID**: `cell-cell-communication`
- **Applicable Scenarios**: Tumor microenvironment, immune cell interactions, tissue niche analysis
- **Key Features**:
  - Ligand-receptor interaction database integration
  - Cell communication network inference and scoring
  - Signaling pathway activity analysis
  - Communication strength visualization (chord diagrams, bubble plots)
  - Differential communication comparison across conditions
- **Dependencies**: CellChat v2, R

---

## 5. GRN pySCENIC

- **Skill ID**: `grn-pyscenic`
- **Applicable Scenarios**: Transcriptional regulatory network research, TF activity analysis
- **Key Features**:
  - Gene regulatory network (GRN) inference from scRNA-seq
  - Cell-level TF activity scoring (AUCell)
  - Regulon identification and visualization
  - Cross-cell-type TF activity comparison
  - Integration with SCENIC+ for multi-omics GRN
- **Dependencies**: pySCENIC, SCENIC+, Python

---

## 6. Spatial Transcriptomics

- **Skill ID**: `spatial-transcriptomics`
- **Applicable Scenarios**: Tissue section spatial gene expression, histology integration
- **Key Features**:
  - 10x Visium data QC and preprocessing
  - Spatial domain identification and clustering
  - Spatially variable gene (SVG) detection
  - Cell type deconvolution (RCTD, SPOTlight)
  - Neighborhood enrichment analysis
  - Spatial visualization overlaid on tissue images
- **Dependencies**: Squidpy, Scanpy, RCTD, Python/R

---

## 7. Pooled CRISPR Screens

- **Skill ID**: `pooled-crispr-screens`
- **Applicable Scenarios**: Functional genomics, gene function characterization, drug target validation
- **Key Features**:
  - Perturb-seq / CROP-seq data processing
  - sgRNA assignment and cell filtering
  - Perturbation effect scoring
  - Differential expression analysis (perturbed vs. control)
  - Gene functional enrichment of screen hits
- **Dependencies**: Pertpy, Scanpy, Python

---

<div align="center">

[← Back to Main Catalog](../README.md) &nbsp;|&nbsp; [中文主页](../README_CN.md) &nbsp;|&nbsp; [Contributing](../CONTRIBUTING.md)

*Part of the [Biomni Skills Catalog](https://github.com/junior1p/biomni-skills-catalog) · Maintained by [Phylo](https://phylo.com)*

</div>
