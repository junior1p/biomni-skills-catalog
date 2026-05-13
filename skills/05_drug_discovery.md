<div align="center">

# 💊 Drug Discovery & Clinical

[![Skills in Category](https://img.shields.io/badge/Skills%20in%20Category-6-4CAF50?style=flat-square)](../README.md)
[![Back to Catalog](https://img.shields.io/badge/Back%20to-Main%20Catalog-blueviolet?style=flat-square)](../README.md)

</div>

---

## Overview

This category covers skills for drug target identification, clinical trial landscape analysis,
preclinical evidence synthesis, biomarker discovery, and clinical survival analysis.

| # | Skill Name | Skill ID |
|---|---|---|
| 1 | Open Targets Platform | `open-targets` |
| 2 | scRNA Disease Drug Discovery | `scrna-disease-drug-discovery` |
| 3 | ClinicalTrials Landscape | `clinicaltrials-landscape` |
| 4 | Literature Preclinical | `literature-preclinical` |
| 5 | LASSO Biomarker Panel | `lasso-biomarker-panel` |
| 6 | Survival Analysis | `survival-analysis-clinical` |

---

## 1. Open Targets Platform

- **Skill ID**: `open-targets`
- **Applicable Scenarios**: Target-disease association analysis, drug target prioritization
- **Key Features**:
  - Target annotations: tractability, essentiality, expression, constraint, safety
  - Disease annotations: ontology, known drugs, associated targets
  - Drug/compound info: mechanism of action, indications, clinical stage, adverse events
  - Target-disease association scores across 20+ datasources
  - Variant and GWAS data: L2G predictions, colocalisation
  - Name → ID resolution for genes, diseases, and drugs
- **API**: GraphQL (https://api.platform.opentargets.org/api/v4/graphql)
- **Data License**: CC0 1.0

---

## 2. scRNA Disease Drug Discovery

- **Skill ID**: `scrna-disease-drug-discovery`
- **Applicable Scenarios**: Disease mechanism research, multi-omics target discovery
- **Key Features**:
  - End-to-end scRNA-seq disease analysis pipeline
  - Disease cell type identification and characterization
  - Genetic evidence integration (GWAS, eQTL, Open Targets)
  - Multi-omics drug target prioritization
  - Target tractability and safety assessment
  - Candidate target report generation
- **Dependencies**: Scanpy, Open Targets API, Python

---

## 3. ClinicalTrials Landscape

- **Skill ID**: `clinicaltrials-landscape`
- **Applicable Scenarios**: Competitive landscape analysis, R&D strategy, market assessment
- **Key Features**:
  - ClinicalTrials.gov API v2 query
  - Filtering by disease area, mechanism, phase, sponsor, and status
  - Clinical trial landscape visualization
  - Trial status and outcome tracking
  - Competitive landscape summary
  - Data export (CSV / Excel)
- **Data Source**: ClinicalTrials.gov

---

## 4. Literature Preclinical

- **Skill ID**: `literature-preclinical`
- **Applicable Scenarios**: Target validation, preclinical evidence synthesis
- **Key Features**:
  - Target-disease preclinical literature search
  - In vivo experiment detail extraction (animal model, dosing, outcomes)
  - In vitro experiment detail extraction (cell line, concentration, endpoints)
  - Structured evidence summary table
  - Evidence strength assessment
- **Data Sources**: PubMed, bioRxiv, EuropePMC

---

## 5. LASSO Biomarker Panel

- **Skill ID**: `lasso-biomarker-panel`
- **Applicable Scenarios**: Diagnostic biomarker development, prognostic model construction
- **Key Features**:
  - LASSO regularization feature selection
  - Nested cross-validation (prevents overfitting)
  - Stability selection (identifies consistently selected features)
  - Independent cohort validation
  - Minimal biomarker panel output
  - Model performance evaluation (AUC, calibration curve, NRI)
- **Dependencies**: glmnet, caret, R

---

## 6. Survival Analysis

- **Skill ID**: `survival-analysis-clinical`
- **Applicable Scenarios**: Clinical prognostic research, survival analysis, risk stratification
- **Key Features**:
  - Kaplan-Meier survival curve estimation
  - Log-rank test for group comparison
  - Cox proportional hazards regression
  - Multivariate survival analysis with covariate adjustment
  - Risk stratification (high / low risk groups)
  - Time-dependent ROC analysis
- **Dependencies**: survival, survminer, R

---

<div align="center">

[← Back to Main Catalog](../README.md) &nbsp;|&nbsp; [中文主页](../README_CN.md) &nbsp;|&nbsp; [Contributing](../CONTRIBUTING.md)

*Part of the [Biomni Skills Catalog](https://github.com/junior1p/biomni-skills-catalog) · Maintained by [Phylo](https://phylo.com)*

</div>
