# 🧪 表观基因组学技能

本目录收录 Biomni 平台中与 ChIP-seq、ATAC-seq、DNA 甲基化等表观基因组学相关的技能。

---

## 1. ChIP-Atlas Peak Enrichment

- **Skill ID**: `chip-atlas-peak-enrichment`
- **适用场景**: 转录因子结合位点分析、组蛋白修饰研究
- **主要功能**:
  - 基于 ChIP-Atlas 43万+ 公开实验数据
  - 用户基因组区域的峰富集分析
  - 跨细胞系/组织类型比较
  - 富集分数计算与排序
  - 结果可视化与导出
- **数据来源**: ChIP-Atlas API (https://chip-atlas.org)

---

## 2. ChIP-Atlas Target Genes

- **Skill ID**: `chip-atlas-target-genes`
- **适用场景**: 转录因子靶基因预测、调控网络构建
- **主要功能**:
  - 获取任意 TF 的预计算靶基因列表
  - 支持按细胞系/组织类型过滤
  - 靶基因置信度评分
  - 与差异表达数据整合
  - 靶基因功能富集分析
- **数据来源**: ChIP-Atlas 预计算数据库

---

## 3. ChIP-Atlas Diff Analysis

- **Skill ID**: `chip-atlas-diff-analysis`
- **适用场景**: 条件间表观遗传差异分析
- **主要功能**:
  - 两组 ChIP-seq/ATAC-seq/DNase-seq 比较
  - 差异峰区域（DPR）识别
  - Bisulfite-seq 差异甲基化区域（DMR）分析
  - 差异区域注释（基因组位置、最近基因）
  - 差异区域可视化
- **数据来源**: ChIP-Atlas API

---

## 4. Upstream Regulator Analysis

- **Skill ID**: `upstream-regulator-analysis`
- **适用场景**: 转录调控机制研究、药物靶点发现
- **主要功能**:
  - 整合 ChIP-Atlas TF 结合数据
  - 与 RNA-seq 差异表达数据联合分析
  - 识别驱动转录组变化的上游调控因子
  - TF 活性评分与排序
  - 调控网络可视化
- **依赖工具**: ChIP-Atlas API, R/Python

---

[← 返回主目录](../README.md)
