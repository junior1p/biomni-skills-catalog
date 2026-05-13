<div align="center">

<img src="https://avatars.githubusercontent.com/u/155460658?v=4" width="120" alt="Biomni Logo" />

# Biomni 技能目录

**[Phylo](https://phylo.bio) 旗下 [Biomni](https://phylo.bio) 平台 AI 驱动研究技能的官方目录。**

*从原始数据到生物学洞见 — 一个技能，一步到位。*

---

[![技能数量](https://img.shields.io/badge/技能-29个-4CAF50?style=flat-square&logo=bookstack&logoColor=white)](https://github.com/junior1p/biomni-skills-catalog)
[![HPC工具](https://img.shields.io/badge/HPC工具-45个-2196F3?style=flat-square&logo=server&logoColor=white)](https://github.com/junior1p/biomni-skills-catalog)
[![许可证](https://img.shields.io/badge/许可证-MIT-yellow?style=flat-square)](LICENSE)
[![最后更新](https://img.shields.io/badge/最后更新-2026--05--14-orange?style=flat-square)](CHANGELOG.md)
[![平台](https://img.shields.io/badge/平台-Biomni%20by%20Phylo-blueviolet?style=flat-square)](https://phylo.bio)

**[English](README.md) | [中文](README_CN.md)**

</div>

---

## 目录

- [平台简介](#平台简介)
- [技能分类](#技能分类)
  - [单细胞与空间转录组](#-单细胞与空间转录组)
  - [批量组学数据分析](#-批量组学数据分析)
  - [表观基因组学](#-表观基因组学)
  - [遗传学与变异分析](#-遗传学与变异分析)
  - [药物发现与临床](#-药物发现与临床)
  - [序列与结构生物学](#-序列与结构生物学)
  - [数据管理与实验设计](#-数据管理与实验设计)
- [HPC 高性能计算工具](#hpc-高性能计算工具)
- [快速开始](#快速开始)
- [贡献指南](#贡献指南)
- [许可证](#许可证)

---

## 平台简介

Biomni 是由 [Phylo](https://phylo.bio) 打造的 AI 驱动生物医学研究平台，将蛋白质模型、生物信息学工具与生成式 AI 整合为统一、易用的研究界面。

本仓库汇总了 Biomni 平台所有可用的**技能（Skills）**——由专家精心设计的可复用分析工作流，每个技能封装了从数据输入到发表级输出的完整分析流程。

| 分类 | 技能数量 |
|---|:---:|
| 单细胞与空间转录组 | 7 |
| 批量组学数据分析 | 6 |
| 表观基因组学 | 4 |
| 遗传学与变异分析 | 4 |
| 药物发现与临床 | 6 |
| 序列与结构生物学 | 1 |
| 数据管理与实验设计 | 3 |
| **合计** | **31** |

---

## 技能分类

### 🔬 单细胞与空间转录组

> 完整文档：[skills/01_single_cell.md](skills/01_single_cell.md)

| 技能名称 | Skill ID | 功能描述 |
|---|---|---|
| scRNAseq Scanpy 核心分析 | `scrnaseq-scanpy-core-analysis` | 基于 Scanpy 的单细胞 RNA-seq 全流程：QC、归一化、聚类、UMAP 与细胞类型注释 |
| scRNAseq Seurat 核心分析 | `scrnaseq-seurat-core-analysis` | 基于 Seurat v5 的单细胞 RNA-seq 全流程：SCTransform、聚类、整合与注释 |
| scRNA 轨迹推断 | `scrna-trajectory-inference` | 拟时序排序、分化轨迹推断、RNA velocity 及细胞命运概率分析 |
| 细胞间通讯 | `cell-cell-communication` | 基于 CellChat v2 的配体-受体互作分析与细胞通讯网络推断 |
| GRN pySCENIC | `grn-pyscenic` | 基于 pySCENIC 的转录因子调控网络推断与细胞水平 TF 活性评分 |
| 空间转录组 | `spatial-transcriptomics` | 10x Visium 全流程：QC、空间域分析、空间变异基因检测与细胞类型去卷积 |
| 汇集 CRISPR 筛选 | `pooled-crispr-screens` | Perturb-seq/CROP-seq 分析：sgRNA 分配、扰动效应评估与差异表达分析 |

---

### 📊 批量组学数据分析

> 完整文档：[skills/02_bulk_omics.md](skills/02_bulk_omics.md)

| 技能名称 | Skill ID | 功能描述 |
|---|---|---|
| Bulk RNA-seq 差异表达 (DESeq2) | `bulk-rnaseq-counts-to-de-deseq2` | 基于 DESeq2 对原始计数矩阵进行差异表达分析，含火山图与 MA 图 |
| 批量组学聚类 | `bulk-omics-clustering` | 转录组、蛋白组、代谢组数据的样本与特征聚类分析 |
| 蛋白组差异表达 | `proteomics-diff-exp` | 基于 limma + DEqMS 的质谱蛋白组学差异分析，支持 PSM 感知方差估计 |
| 多组学整合 | `multi-omics-integration` | 基于 MOFA+ 整合 2+ 组学层，进行潜在因子分解与跨组学方差分析 |
| 功能富集分析 | `functional-enrichment-from-degs` | 基于 clusterProfiler 对差异表达结果进行 GO/KEGG/Reactome 富集（ORA + GSEA） |
| 共表达网络 | `coexpression-network` | 基于 WGCNA 构建基因共表达网络，识别功能模块与枢纽基因 |

---

### 🧪 表观基因组学

> 完整文档：[skills/03_epigenomics.md](skills/03_epigenomics.md)

| 技能名称 | Skill ID | 功能描述 |
|---|---|---|
| ChIP-Atlas 峰富集分析 | `chip-atlas-peak-enrichment` | 基于 ChIP-Atlas 43万+ 公开实验的 ChIP-seq 峰富集分析 |
| ChIP-Atlas 靶基因 | `chip-atlas-target-genes` | 从 ChIP-Atlas 公开数据获取任意转录因子的预计算靶基因列表 |
| ChIP-Atlas 差异分析 | `chip-atlas-diff-analysis` | 两组 ChIP/ATAC/DNase-seq 或 Bisulfite-seq 比较，识别差异峰区域或差异甲基化区域 |
| 上游调控因子分析 | `upstream-regulator-analysis` | 整合 ChIP-Atlas TF 结合数据与 RNA-seq 差异表达，识别上游转录调控因子 |

---

### 🧬 遗传学与变异分析

> 完整文档：[skills/04_genetics.md](skills/04_genetics.md)

| 技能名称 | Skill ID | 功能描述 |
|---|---|---|
| 基因组变异注释 | `genetic-variant-annotation` | 对 VCF 变异进行功能效应、临床意义（ClinVar）与致病性预测注释 |
| GWAS 到功能 (TWAS) | `gwas-to-function-twas` | 利用转录组全关联研究（TWAS）从 GWAS 数据识别因果基因与治疗靶点 |
| 孟德尔随机化 | `mendelian-randomization-twosamplemr` | 基于 GWAS 汇总统计的两样本孟德尔随机化因果推断（IVW、MR-Egger、WM、PRESSO） |
| 多基因风险评分 | `polygenic-risk-score-prs-catalog` | 利用 PGS Catalog 预计算权重计算 PRS，支持人群比较与风险分层 |

---

### 💊 药物发现与临床

> 完整文档：[skills/05_drug_discovery.md](skills/05_drug_discovery.md)

| 技能名称 | Skill ID | 功能描述 |
|---|---|---|
| Open Targets 平台 | `open-targets` | 通过 Open Targets GraphQL API 查询靶点-疾病关联、药物注释与 GWAS 证据 |
| scRNA 疾病药物发现 | `scrna-disease-drug-discovery` | 端到端单细胞 RNA-seq 疾病分析，整合遗传证据进行多组学靶点优先排序 |
| 临床试验全景图 | `clinicaltrials-landscape` | 基于 ClinicalTrials.gov API v2，按机制、阶段和申办方绘制临床试验全景图 |
| 临床前文献挖掘 | `literature-preclinical` | 从临床前文献中提取任意靶点的结构化体内/体外实验详情 |
| LASSO 生物标志物面板 | `lasso-biomarker-panel` | 基于 LASSO 正则化、嵌套交叉验证与稳定性选择筛选最小生物标志物面板 |
| 生存分析 | `survival-analysis-clinical` | 对临床时间-事件数据进行 Kaplan-Meier 估计、Cox 回归与风险分层 |

---

### 🔗 序列与结构生物学

> 完整文档：[skills/06_other_skills.md](skills/06_other_skills.md)

| 技能名称 | Skill ID | 功能描述 |
|---|---|---|
| PCR 引物设计 | `pcr-primer-design` | 设计并验证 PCR、qPCR、TaqMan 和测序引物，含 BLAST 特异性检查 |

---

### 📁 数据管理与实验设计

> 完整文档：[skills/06_other_skills.md](skills/06_other_skills.md)

| 技能名称 | Skill ID | 功能描述 |
|---|---|---|
| 组学数据集检索 | `omics-dataset-retrieval` | 从 GEO、ArrayExpress、ENCODE、SRA 等数据库检索和整理公开组学数据集 |
| 实验设计统计 | `experimental-design-statistics` | 基因组学实验功效分析、样本量估算、批次设计与多重检验校正 |
| 疾病进展纵向分析 | `disease-progression-longitudinal` | 从纵向患者组学数据重建疾病进展轨迹 |

---

## HPC 高性能计算工具

除技能外，Biomni 还提供 **45 个高性能计算工具**，适用于计算密集型生物信息学任务：

| 类别 | 工具 |
|---|---|
| **基因组组装** | Canu · Flye · hifiasm · MEGAHIT · NextDenovo · Raven · SPAdes · Unicycler · Verkko · wtdbg2 |
| **变异检测** | BCFtools · Clair3 · FreeBayes · Longshot · NanoCaller · PEPPER-DeepVariant · Sniffles · Strelka2 |
| **RNA-seq 与定量** | HISAT2 · Kallisto · Salmon · STAR · STAR-Fusion · StringTie · Trinity |
| **蛋白质结构与设计** | AlphaFold v2 · Boltz-2 · BoltzGen · Chai-1 · Foldseek · ImmuneBuilder · ProteinMPNN · RFAntibody · RFDiffusion · ThermoMPNN |
| **序列比对** | DIAMOND · minimap2 · MMseqs2 |
| **基因组注释** | Bakta · Prokka |
| **单细胞** | CellBender · Cellpose |
| **质量控制** | CheckM2 · MultiQC · QUAST |

---

## 快速开始

技能直接在 Biomni 平台内调用，示例如下：

```python
# 按名称或 ID 加载技能
Skill(action="load", name="scrnaseq-scanpy-core-analysis")

# 或按 Skill ID 加载
Skill(action="load", name="skill_e4c50152a70f4d6fa8a4802573755f54")
```

加载后，技能将提供针对你数据的逐步指导、代码模板和最佳实践。

**示例 — 差异表达分析：**

```python
# 1. 加载 DESeq2 技能
Skill(action="load", name="bulk-rnaseq-counts-to-de-deseq2")

# 2. 技能将引导你完成：
#    - 加载计数矩阵
#    - 设置 DESeq2 设计公式
#    - 运行差异表达分析
#    - 生成火山图和结果表格
```

---

## 贡献指南

欢迎贡献以改进和扩展本目录。请阅读 [CONTRIBUTING.md](CONTRIBUTING.md) 了解：

- 如何添加新技能
- 文档格式规范
- Pull Request 流程

---

## 许可证

本项目采用 [MIT 许可证](LICENSE)。

---

<div align="center">

由 [Phylo](https://phylo.bio) 团队用心打造 · 最后更新：2026-05-14

*以 AI 赋能生物医学研究*

</div>
