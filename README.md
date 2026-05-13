# 🧬 Biomni Skills Catalog

> **Biomni** 是由 [Phylo](https://phylo.com) 打造的 AI 驱动生物医学研究平台，集成蛋白质模型、生物信息学工具与生成式 AI，为科研人员提供一站式智能分析能力。

本仓库汇总了 Biomni 平台目前所有可用的**技能（Skills）**，覆盖从原始数据处理到药物发现的完整生物医学研究流程。

---

## 📚 技能分类总览

| 分类 | 技能数量 |
|------|---------|
| [🔬 单细胞与空间转录组](#-单细胞与空间转录组) | 6 |
| [📊 批量组学数据分析](#-批量组学数据分析) | 5 |
| [🧪 表观基因组学](#-表观基因组学) | 4 |
| [🧬 遗传学与变异分析](#-遗传学与变异分析) | 4 |
| [💊 药物发现与临床](#-药物发现与临床) | 6 |
| [🔗 序列与结构生物学](#-序列与结构生物学) | 1 |
| [📁 数据管理与实验设计](#-数据管理与实验设计) | 3 |

**合计：29 个专业技能**

---

## 🔬 单细胞与空间转录组

| 技能名称 | Skill ID | 功能描述 |
|---------|----------|---------|
| scRNAseq Scanpy Core Analysis | `scrnaseq-scanpy-core-analysis` | 基于 Scanpy 的单细胞 RNA-seq 全流程分析，从原始数据到细胞类型注释、聚类与可视化 |
| scRNAseq Seurat Core Analysis | `scrnaseq-seurat-core-analysis` | 基于 Seurat 的单细胞 RNA-seq 全流程分析，从原始数据到细胞类型注释、聚类与可视化 |
| scRNA Trajectory Inference | `scrna-trajectory-inference` | 分化轨迹推断、拟时序排序、RNA velocity 及细胞命运概率分析 |
| Cell-Cell Communication | `cell-cell-communication` | 基于 CellChat v2 配体-受体互作分析，推断并可视化细胞间通讯网络 |
| GRN pySCENIC | `grn-pyscenic` | 基于 pySCENIC 从单细胞 RNA-seq 数据推断转录因子调控网络及细胞水平 TF 活性 |
| Spatial Transcriptomics | `spatial-transcriptomics` | 10x Visium 空间转录组全流程分析，含 QC、空间域分析、聚类、空间变异基因及邻域富集 |
| Pooled CRISPR Screens | `pooled-crispr-screens` | 带单细胞 RNA-seq 读出的 CRISPR 筛选分析（Perturb-seq/CROP-seq） |

---

## 📊 批量组学数据分析

| 技能名称 | Skill ID | 功能描述 |
|---------|----------|---------|
| Bulk RNA-seq Counts to DE (DESeq2) | `bulk-rnaseq-counts-to-de-deseq2` | 基于 DESeq2 对 RNA-seq 原始计数数据进行差异表达分析 |
| Bulk Omics Clustering | `bulk-omics-clustering` | 批量转录组/蛋白组/代谢组数据的样本或特征聚类分析 |
| Proteomics Diff Exp | `proteomics-diff-exp` | 基于 limma + DEqMS 的质谱蛋白组学差异表达分析，支持 PSM 感知方差估计 |
| Multi-Omics Integration | `multi-omics-integration` | 基于 MOFA+ 整合 2+ 组学层，识别跨组学变异的潜在因子，含方差分解与因子解读 |
| Functional Enrichment from DEGs | `functional-enrichment-from-degs` | 基于 clusterProfiler 对差异表达基因进行功能富集分析（GSEA + ORA） |
| Co-expression Network | `coexpression-network` | 构建基因共表达网络，识别功能模块和枢纽基因 |

---

## 🧪 表观基因组学

| 技能名称 | Skill ID | 功能描述 |
|---------|----------|---------|
| ChIP-Atlas Peak Enrichment | `chip-atlas-peak-enrichment` | 基于 ChIP-Atlas 43万+实验数据分析 ChIP-seq 峰富集 |
| ChIP-Atlas Target Genes | `chip-atlas-target-genes` | 从 ChIP-Atlas 公开 ChIP-seq 数据获取任意转录因子的预计算靶基因 |
| ChIP-Atlas Diff Analysis | `chip-atlas-diff-analysis` | 比较两组 ChIP/ATAC/DNase-seq 或 Bisulfite-seq 实验，识别差异峰区域（DPR）或差异甲基化区域（DMR） |
| Upstream Regulator Analysis | `upstream-regulator-analysis` | 整合 ChIP-Atlas TF 结合数据与 RNA-seq 差异表达，识别驱动转录组变化的上游调控因子 |

---

## 🧬 遗传学与变异分析

| 技能名称 | Skill ID | 功能描述 |
|---------|----------|---------|
| Genetic Variant Annotation | `genetic-variant-annotation` | 对 VCF 文件中的基因组变异进行功能效应、临床意义和致病性预测注释 |
| GWAS to Function (TWAS) | `gwas-to-function-twas` | 利用转录组全关联研究（TWAS）从 GWAS 数据识别因果基因和治疗靶点 |
| Mendelian Randomization | `mendelian-randomization-twosamplemr` | 基于 GWAS 汇总统计和遗传工具变量进行孟德尔随机化因果推断 |
| Polygenic Risk Score (PRS Catalog) | `polygenic-risk-score-prs-catalog` | 利用 PGS Catalog 预计算权重计算单个或多个性状的多基因风险评分，支持人群比较 |

---

## 💊 药物发现与临床

| 技能名称 | Skill ID | 功能描述 |
|---------|----------|---------|
| Open Targets Platform | `open-targets` | 通过 GraphQL API 查询 Open Targets 靶点-疾病关联、证据和注释，支持药物靶点识别 |
| scRNA Disease Drug Discovery | `scrna-disease-drug-discovery` | 端到端单细胞 RNA-seq 疾病分析，整合遗传证据进行多组学药物靶点优先排序 |
| ClinicalTrials Landscape | `clinicaltrials-landscape` | 查询 ClinicalTrials.gov API v2，按机制、阶段和申办方绘制疾病领域临床试验全景图 |
| Literature Preclinical | `literature-preclinical` | 搜索靶点在疾病中的临床前研究，从每篇文献中提取结构化体内外实验详情 |
| LASSO Biomarker Panel | `lasso-biomarker-panel` | 使用 LASSO 正则化结合嵌套交叉验证、稳定性选择和独立队列验证，筛选最小生物标志物面板 |
| Survival Analysis Clinical | `survival-analysis-clinical` | 对临床时间-事件数据进行 Kaplan-Meier 估计、Cox 比例风险回归和风险分层 |

---

## 🔗 序列与结构生物学

| 技能名称 | Skill ID | 功能描述 |
|---------|----------|---------|
| PCR Primer Design | `pcr-primer-design` | 设计并验证 PCR、qPCR、TaqMan 和测序应用的引物 |

---

## 📁 数据管理与实验设计

| 技能名称 | Skill ID | 功能描述 |
|---------|----------|---------|
| Omics Dataset Retrieval | `omics-dataset-retrieval` | 从 GEO、ArrayExpress 等公开数据库检索和整理组学数据集 |
| Experimental Design Statistics | `experimental-design-statistics` | 基因组学实验功效分析、样本量估算、批次设计和多重检验校正 |
| Disease Progression Longitudinal | `disease-progression-longitudinal` | 从纵向患者组学数据重建疾病进展轨迹 |

---

## 🚀 如何使用技能

在 Biomni 平台中，可以通过以下方式调用技能：

```python
# 加载技能
Skill(action="load", name="<skill_name_or_id>")

# 示例：加载单细胞分析技能
Skill(action="load", name="scrnaseq-scanpy-core-analysis")
```

---

## 🔧 HPC 工具（高性能计算）

除技能外，平台还支持以下 HPC 工具，适用于计算密集型生物信息学任务：

`AlphaFold v2` · `Bakta` · `BCFtools` · `Boltz-2` · `BoltzGen` · `Canu` · `CellBender` · `Cellpose` · `Chai-1` · `CheckM2` · `Clair3` · `DIAMOND` · `Flye` · `Foldseek` · `FreeBayes` · `hifiasm` · `HISAT2` · `ImmuneBuilder` · `Kallisto` · `Longshot` · `MEGAHIT` · `minimap2` · `MMseqs2` · `MultiQC` · `NanoCaller` · `NextDenovo` · `PEPPER-DeepVariant` · `Prokka` · `ProteinMPNN` · `QUAST` · `Raven` · `RFAntibody` · `RFDiffusion` · `Salmon` · `Sniffles` · `SPAdes` · `STAR` · `STAR-Fusion` · `Strelka2` · `StringTie` · `ThermoMPNN` · `Trinity` · `Unicycler` · `Verkko` · `wtdbg2`

---

## 📅 更新记录

| 日期 | 内容 |
|------|------|
| 2026-05-14 | 初始版本，汇总 29 个技能 |

---

> 由 [Biomni (Phylo)](https://phylo.com) 自动生成 · 最后更新：2026-05-14
