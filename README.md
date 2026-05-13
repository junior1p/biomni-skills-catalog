<div align="center">

<img src="https://biomni.phylo.bio/biomni_logo_icon.png" width="120" alt="Biomni by Phylo" />

# Biomni Skills Catalog

**The official catalog of AI-powered research skills for the [Biomni](https://phylo.bio) platform by Phylo.**

*From raw data to biological insight — one skill at a time.*

---

[![Skills](https://img.shields.io/badge/Skills-29-4CAF50?style=flat-square&logo=bookstack&logoColor=white)](https://github.com/junior1p/biomni-skills-catalog)
[![HPC Tools](https://img.shields.io/badge/HPC%20Tools-45-2196F3?style=flat-square&logo=server&logoColor=white)](https://github.com/junior1p/biomni-skills-catalog)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)
[![Last Updated](https://img.shields.io/badge/Last%20Updated-2026--05--14-orange?style=flat-square)](CHANGELOG.md)
[![Platform](https://img.shields.io/badge/Platform-Biomni%20by%20Phylo-blueviolet?style=flat-square)](https://phylo.bio)

**[English](README.md) | [中文](README_CN.md)**

</div>

---

## Table of Contents

- [Overview](#overview)
- [Skills by Category](#skills-by-category)
  - [Single-Cell & Spatial Transcriptomics](#-single-cell--spatial-transcriptomics)
  - [Bulk Omics Analysis](#-bulk-omics-analysis)
  - [Epigenomics](#-epigenomics)
  - [Genetics & Variant Analysis](#-genetics--variant-analysis)
  - [Drug Discovery & Clinical](#-drug-discovery--clinical)
  - [Sequence & Structural Biology](#-sequence--structural-biology)
  - [Data Management & Experimental Design](#-data-management--experimental-design)
- [HPC Tools](#hpc-tools)
- [Quick Start](#quick-start)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

Biomni is an AI-powered biomedical research platform built by [Phylo](https://phylo.bio). It integrates protein models, bioinformatics tools, and generative AI into a unified, accessible interface.

This repository catalogs all **Skills** — reusable, expert-curated analytical workflows — available on the Biomni platform. Each skill encapsulates a complete analysis pipeline, from data ingestion to publication-ready outputs.

| Category | Skills |
|---|:---:|
| Single-Cell & Spatial Transcriptomics | 7 |
| Bulk Omics Analysis | 6 |
| Epigenomics | 4 |
| Genetics & Variant Analysis | 4 |
| Drug Discovery & Clinical | 6 |
| Sequence & Structural Biology | 1 |
| Data Management & Experimental Design | 3 |
| **Total** | **31** |

---

## Skills by Category

### 🔬 Single-Cell & Spatial Transcriptomics

> Full documentation: [skills/01_single_cell.md](skills/01_single_cell.md)

| Skill Name | Skill ID | Description |
|---|---|---|
| scRNAseq Scanpy Core Analysis | `scrnaseq-scanpy-core-analysis` | Complete scRNA-seq pipeline using Scanpy: QC, normalization, clustering, UMAP, and cell type annotation |
| scRNAseq Seurat Core Analysis | `scrnaseq-seurat-core-analysis` | Complete scRNA-seq pipeline using Seurat v5: SCTransform, clustering, integration, and annotation |
| scRNA Trajectory Inference | `scrna-trajectory-inference` | Pseudotime ordering, differentiation trajectory inference, RNA velocity, and cell fate probabilities |
| Cell-Cell Communication | `cell-cell-communication` | Ligand-receptor interaction analysis and cell communication network inference using CellChat v2 |
| GRN pySCENIC | `grn-pyscenic` | Transcription factor regulatory network inference and cell-level TF activity scoring via pySCENIC |
| Spatial Transcriptomics | `spatial-transcriptomics` | 10x Visium spatial transcriptomics: QC, spatial domain analysis, SVG detection, and deconvolution |
| Pooled CRISPR Screens | `pooled-crispr-screens` | Perturb-seq/CROP-seq analysis: sgRNA assignment, perturbation effect scoring, and DEG analysis |

---

### 📊 Bulk Omics Analysis

> Full documentation: [skills/02_bulk_omics.md](skills/02_bulk_omics.md)

| Skill Name | Skill ID | Description |
|---|---|---|
| Bulk RNA-seq DE (DESeq2) | `bulk-rnaseq-counts-to-de-deseq2` | Differential expression analysis from raw count matrices using DESeq2 with volcano/MA plots |
| Bulk Omics Clustering | `bulk-omics-clustering` | Sample and feature clustering for transcriptomics, proteomics, and metabolomics data |
| Proteomics Diff Exp | `proteomics-diff-exp` | Mass spectrometry proteomics differential analysis using limma + DEqMS with PSM-aware variance |
| Multi-Omics Integration | `multi-omics-integration` | Integrate 2+ omics layers using MOFA+ for latent factor decomposition and cross-omics variance analysis |
| Functional Enrichment | `functional-enrichment-from-degs` | GO/KEGG/Reactome enrichment (ORA + GSEA) using clusterProfiler on differential expression results |
| Co-expression Network | `coexpression-network` | WGCNA-based gene co-expression network construction, module identification, and hub gene discovery |

---

### 🧪 Epigenomics

> Full documentation: [skills/03_epigenomics.md](skills/03_epigenomics.md)

| Skill Name | Skill ID | Description |
|---|---|---|
| ChIP-Atlas Peak Enrichment | `chip-atlas-peak-enrichment` | ChIP-seq peak enrichment analysis against 433,000+ public experiments via ChIP-Atlas API |
| ChIP-Atlas Target Genes | `chip-atlas-target-genes` | Retrieve pre-computed TF target gene lists from ChIP-Atlas public ChIP-seq data |
| ChIP-Atlas Diff Analysis | `chip-atlas-diff-analysis` | Differential peak regions (DPR) or differentially methylated regions (DMR) between two conditions |
| Upstream Regulator Analysis | `upstream-regulator-analysis` | Integrate ChIP-Atlas TF binding with RNA-seq DE to identify upstream transcriptional regulators |

---

### 🧬 Genetics & Variant Analysis

> Full documentation: [skills/04_genetics.md](skills/04_genetics.md)

| Skill Name | Skill ID | Description |
|---|---|---|
| Genetic Variant Annotation | `genetic-variant-annotation` | Annotate VCF variants with functional effects, clinical significance (ClinVar), and pathogenicity |
| GWAS to Function (TWAS) | `gwas-to-function-twas` | Identify causal genes and therapeutic targets from GWAS using transcriptome-wide association studies |
| Mendelian Randomization | `mendelian-randomization-twosamplemr` | Two-sample MR causal inference using GWAS summary statistics (IVW, MR-Egger, WM, PRESSO) |
| Polygenic Risk Score | `polygenic-risk-score-prs-catalog` | Calculate PRS using PGS Catalog pre-computed weights with population comparison and risk stratification |

---

### 💊 Drug Discovery & Clinical

> Full documentation: [skills/05_drug_discovery.md](skills/05_drug_discovery.md)

| Skill Name | Skill ID | Description |
|---|---|---|
| Open Targets Platform | `open-targets` | Query target–disease associations, drug annotations, and GWAS evidence via Open Targets GraphQL API |
| scRNA Disease Drug Discovery | `scrna-disease-drug-discovery` | End-to-end scRNA-seq disease analysis with genetic evidence integration for target prioritization |
| ClinicalTrials Landscape | `clinicaltrials-landscape` | Map clinical trial landscape by mechanism, phase, and sponsor using ClinicalTrials.gov API v2 |
| Literature Preclinical | `literature-preclinical` | Extract structured in vitro/in vivo experiment details from preclinical literature for any target |
| LASSO Biomarker Panel | `lasso-biomarker-panel` | Minimal biomarker panel selection using LASSO with nested CV, stability selection, and cohort validation |
| Survival Analysis | `survival-analysis-clinical` | Kaplan-Meier estimation, Cox regression, and risk stratification from clinical time-to-event data |

---

### 🔗 Sequence & Structural Biology

> Full documentation: [skills/06_other_skills.md](skills/06_other_skills.md)

| Skill Name | Skill ID | Description |
|---|---|---|
| PCR Primer Design | `pcr-primer-design` | Design and validate primers for PCR, qPCR, TaqMan, and sequencing with BLAST specificity checks |

---

### 📁 Data Management & Experimental Design

> Full documentation: [skills/06_other_skills.md](skills/06_other_skills.md)

| Skill Name | Skill ID | Description |
|---|---|---|
| Omics Dataset Retrieval | `omics-dataset-retrieval` | Search and catalog public omics datasets from GEO, ArrayExpress, ENCODE, and SRA |
| Experimental Design Statistics | `experimental-design-statistics` | Power analysis, sample size estimation, batch design, and multiple testing correction for genomics |
| Disease Progression Longitudinal | `disease-progression-longitudinal` | Reconstruct disease progression trajectories from longitudinal patient omics data |

---

## HPC Tools

In addition to Skills, Biomni provides access to **45 high-performance computing tools** for computationally intensive bioinformatics tasks:

| Category | Tools |
|---|---|
| **Genome Assembly** | Canu · Flye · hifiasm · MEGAHIT · NextDenovo · Raven · SPAdes · Unicycler · Verkko · wtdbg2 |
| **Variant Calling** | BCFtools · Clair3 · FreeBayes · Longshot · NanoCaller · PEPPER-DeepVariant · Sniffles · Strelka2 |
| **RNA-seq & Quantification** | HISAT2 · Kallisto · Salmon · STAR · STAR-Fusion · StringTie · Trinity |
| **Protein Structure & Design** | AlphaFold v2 · Boltz-2 · BoltzGen · Chai-1 · Foldseek · ImmuneBuilder · ProteinMPNN · RFAntibody · RFDiffusion · ThermoMPNN |
| **Sequence Alignment** | DIAMOND · minimap2 · MMseqs2 |
| **Genome Annotation** | Bakta · Prokka |
| **Single-Cell** | CellBender · Cellpose |
| **Quality Control** | CheckM2 · MultiQC · QUAST |

---

## Quick Start

Skills are invoked directly within the Biomni platform. Here is an example of how to load and use a skill:

```python
# Load a skill by name or ID
Skill(action="load", name="scrnaseq-scanpy-core-analysis")

# Or load by skill ID
Skill(action="load", name="skill_e4c50152a70f4d6fa8a4802573755f54")
```

Once loaded, the skill provides step-by-step guidance, code templates, and best practices tailored to your data.

**Example — Differential Expression Analysis:**

```python
# 1. Load the DESeq2 skill
Skill(action="load", name="bulk-rnaseq-counts-to-de-deseq2")

# 2. The skill will guide you through:
#    - Loading your count matrix
#    - Setting up the DESeq2 design formula
#    - Running differential expression
#    - Generating volcano plots and result tables
```

---

## Contributing

We welcome contributions to improve and expand this catalog. Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on:

- Adding new skills
- Updating existing skill documentation
- Reporting issues

---

## License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">

Built with care by the [Phylo](https://phylo.bio) team · Last updated: 2026-05-14

*Empowering biomedical research with AI*

</div>
