<div align="center">

# 🧬 Genetics & Variant Analysis

[![Skills in Category](https://img.shields.io/badge/Skills%20in%20Category-4-4CAF50?style=flat-square)](../README.md)
[![Back to Catalog](https://img.shields.io/badge/Back%20to-Main%20Catalog-blueviolet?style=flat-square)](../README.md)

</div>

---

## Overview

This category covers skills for genomic variant annotation, GWAS functional interpretation,
Mendelian randomization causal inference, and polygenic risk score calculation.

| # | Skill Name | Skill ID |
|---|---|---|
| 1 | Genetic Variant Annotation | `genetic-variant-annotation` |
| 2 | GWAS to Function (TWAS) | `gwas-to-function-twas` |
| 3 | Mendelian Randomization | `mendelian-randomization-twosamplemr` |
| 4 | Polygenic Risk Score | `polygenic-risk-score-prs-catalog` |

---

## 1. Genetic Variant Annotation

- **Skill ID**: `genetic-variant-annotation`
- **Applicable Scenarios**: Clinical variant interpretation, functional genomics
- **Key Features**:
  - VCF file input and processing
  - Functional effect prediction (SIFT, PolyPhen-2, CADD, REVEL)
  - Clinical significance annotation (ClinVar, OMIM)
  - Pathogenicity classification (ACMG/AMP criteria)
  - Population frequency annotation (gnomAD, 1000 Genomes)
  - Variant prioritization and ranking
- **Dependencies**: VEP, ANNOVAR, SnpEff

---

## 2. GWAS to Function (TWAS)

- **Skill ID**: `gwas-to-function-twas`
- **Applicable Scenarios**: Complex disease genetic mechanism dissection, therapeutic target discovery
- **Key Features**:
  - GWAS summary statistics input
  - Transcriptome-wide association study (TWAS) analysis
  - Causal gene prioritization
  - Tissue-specific analysis using GTEx expression weights
  - Fine-mapping (SuSiE, FINEMAP)
  - Therapeutic target candidate gene list output
- **Dependencies**: FUSION, PrediXcan, S-PrediXcan, R

---

## 3. Mendelian Randomization

- **Skill ID**: `mendelian-randomization-twosamplemr`
- **Applicable Scenarios**: Exposure-outcome causal relationship research, epidemiology
- **Key Features**:
  - Two-sample Mendelian randomization (2SMR)
  - Instrument variable selection (F-statistic, LD clumping)
  - Multiple MR methods: IVW, MR-Egger, Weighted Median, MR-PRESSO
  - Horizontal pleiotropy testing (Egger intercept, MR-PRESSO)
  - Sensitivity analysis (leave-one-out, funnel plot)
  - Causal effect estimation and visualization
- **Dependencies**: TwoSampleMR, MendelianRandomization, R

---

## 4. Polygenic Risk Score

- **Skill ID**: `polygenic-risk-score-prs-catalog`
- **Applicable Scenarios**: Disease risk prediction, precision medicine, population stratification
- **Key Features**:
  - PGS Catalog pre-computed weight download and application
  - Single or multi-trait PRS calculation
  - Population reference distribution comparison
  - Risk stratification and percentile calculation
  - PRS performance evaluation (AUC, R², calibration)
  - Multi-trait PRS integration
- **Dependencies**: pgscatalog-utils, PLINK2, R

---

<div align="center">

[← Back to Main Catalog](../README.md) &nbsp;|&nbsp; [中文主页](../README_CN.md) &nbsp;|&nbsp; [Contributing](../CONTRIBUTING.md)

*Part of the [Biomni Skills Catalog](https://github.com/junior1p/biomni-skills-catalog) · Maintained by [Phylo](https://phylo.com)*

</div>
