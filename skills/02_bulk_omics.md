# 📊 批量组学数据分析技能

本目录收录 Biomni 平台中与批量转录组、蛋白组、代谢组等组学数据分析相关的技能。

---

## 1. Bulk RNA-seq Counts to DE (DESeq2)

- **Skill ID**: `bulk-rnaseq-counts-to-de-deseq2`
- **适用场景**: 批量 RNA-seq 差异表达分析
- **主要功能**:
  - 原始计数矩阵输入
  - DESeq2 归一化（size factor 估计）
  - 差异表达分析（Wald test / LRT）
  - 多重检验校正（BH-FDR）
  - 火山图、MA 图可视化
  - 差异基因列表输出
- **依赖工具**: DESeq2, R/Bioconductor

---

## 2. Bulk Omics Clustering

- **Skill ID**: `bulk-omics-clustering`
- **适用场景**: 样本分组、亚型发现、质控
- **主要功能**:
  - 层次聚类（Ward, complete linkage）
  - k-means / PAM 聚类
  - PCA / UMAP 降维可视化
  - 热图（ComplexHeatmap）
  - 样本相关性矩阵
  - 批次效应评估
- **依赖工具**: ComplexHeatmap, factoextra, R

---

## 3. Proteomics Diff Exp

- **Skill ID**: `proteomics-diff-exp`
- **适用场景**: 质谱蛋白组学差异蛋白分析
- **主要功能**:
  - MaxQuant/Proteome Discoverer 输出处理
  - PSM 感知方差估计（DEqMS）
  - limma 线性模型差异分析
  - 缺失值处理（MinProb/KNN 插补）
  - 蛋白丰度归一化
  - 差异蛋白可视化
- **依赖工具**: limma, DEqMS, R

---

## 4. Multi-Omics Integration

- **Skill ID**: `multi-omics-integration`
- **适用场景**: 多组学联合分析、生物标志物发现
- **主要功能**:
  - 支持转录组 + 蛋白组 + 代谢组等多层整合
  - MOFA+ 潜在因子分解
  - 跨组学方差分解
  - 因子生物学解读
  - 样本分层与亚型发现
- **依赖工具**: MOFA+, mofapy2, Python/R

---

## 5. Functional Enrichment from DEGs

- **Skill ID**: `functional-enrichment-from-degs`
- **适用场景**: 差异基因功能解读、通路分析
- **主要功能**:
  - 过表示分析（ORA）：GO、KEGG、Reactome
  - 基因集富集分析（GSEA）
  - MSigDB 基因集支持
  - 富集结果可视化（点图、条形图、网络图）
  - 多条件比较富集
- **依赖工具**: clusterProfiler, enrichplot, R

---

## 6. Co-expression Network

- **Skill ID**: `coexpression-network`
- **适用场景**: 基因功能模块发现、枢纽基因识别
- **主要功能**:
  - WGCNA 加权共表达网络构建
  - 模块识别与特征基因提取
  - 模块-性状关联分析
  - 枢纽基因（Hub gene）识别
  - 网络可视化（Cytoscape 兼容输出）
- **依赖工具**: WGCNA, R

---

[← 返回主目录](../README.md)
