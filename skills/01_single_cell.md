# 🔬 单细胞与空间转录组技能

本目录收录 Biomni 平台中与单细胞测序和空间转录组相关的所有技能。

---

## 1. scRNAseq Scanpy Core Analysis

- **Skill ID**: `scrnaseq-scanpy-core-analysis`
- **适用场景**: 10x Genomics、Smart-seq2 等单细胞 RNA-seq 数据
- **主要功能**:
  - 数据质控（QC）：过滤低质量细胞和基因
  - 归一化与对数变换
  - 高变基因筛选、PCA 降维
  - 邻域图构建、UMAP/t-SNE 可视化
  - Leiden/Louvain 聚类
  - 差异表达基因识别
  - 细胞类型自动注释
- **依赖工具**: Scanpy, AnnData, scvi-tools

---

## 2. scRNAseq Seurat Core Analysis

- **Skill ID**: `scrnaseq-seurat-core-analysis`
- **适用场景**: 10x Genomics、Drop-seq 等单细胞 RNA-seq 数据
- **主要功能**:
  - 数据质控与过滤
  - SCTransform 归一化
  - PCA、UMAP 降维与可视化
  - 图聚类（FindClusters）
  - 差异表达分析（FindMarkers）
  - 细胞类型注释
  - 多样本整合（Harmony/CCA）
- **依赖工具**: Seurat v5, R

---

## 3. scRNA Trajectory Inference

- **Skill ID**: `scrna-trajectory-inference`
- **适用场景**: 发育生物学、细胞分化、干细胞研究
- **主要功能**:
  - 拟时序（Pseudotime）排序
  - 分化轨迹推断（Monocle3/PAGA）
  - RNA velocity 分析（scVelo）
  - 细胞命运概率估计（CellRank）
  - 轨迹相关差异基因识别
- **依赖工具**: Monocle3, scVelo, CellRank, PAGA

---

## 4. Cell-Cell Communication

- **Skill ID**: `cell-cell-communication`
- **适用场景**: 组织微环境、免疫细胞互作、肿瘤微环境研究
- **主要功能**:
  - 配体-受体互作数据库整合
  - 细胞间通讯网络推断
  - 信号通路活性分析
  - 通讯强度可视化（弦图、气泡图）
  - 差异通讯比较（多条件）
- **依赖工具**: CellChat v2

---

## 5. GRN pySCENIC

- **Skill ID**: `grn-pyscenic`
- **适用场景**: 转录调控网络研究、转录因子活性分析
- **主要功能**:
  - 转录因子调控网络（GRN）推断
  - 细胞水平 TF 活性评分（AUCell）
  - Regulon 识别与可视化
  - 跨细胞类型 TF 活性比较
- **依赖工具**: pySCENIC, SCENIC+

---

## 6. Spatial Transcriptomics

- **Skill ID**: `spatial-transcriptomics`
- **适用场景**: 组织切片空间基因表达研究
- **主要功能**:
  - 10x Visium 数据 QC 与预处理
  - 空间域识别与聚类
  - 空间变异基因（SVG）检测
  - 细胞类型去卷积
  - 邻域富集分析
  - 空间可视化
- **依赖工具**: Squidpy, Scanpy, RCTD

---

## 7. Pooled CRISPR Screens

- **Skill ID**: `pooled-crispr-screens`
- **适用场景**: 功能基因组学筛选、基因功能研究
- **主要功能**:
  - Perturb-seq/CROP-seq 数据处理
  - sgRNA 分配与细胞过滤
  - 扰动效应评估
  - 差异表达分析（扰动 vs 对照）
  - 基因功能富集
- **依赖工具**: Pertpy, Scanpy

---

[← 返回主目录](../README.md)
