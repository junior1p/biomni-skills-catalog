# 🧬 遗传学与变异分析技能

本目录收录 Biomni 平台中与基因组变异、GWAS、孟德尔随机化和多基因风险评分相关的技能。

---

## 1. Genetic Variant Annotation

- **Skill ID**: `genetic-variant-annotation`
- **适用场景**: 临床变异解读、功能基因组学
- **主要功能**:
  - VCF 文件输入处理
  - 功能效应预测（SIFT, PolyPhen-2, CADD）
  - 临床意义注释（ClinVar, OMIM）
  - 致病性分类（ACMG 标准）
  - 人群频率注释（gnomAD, 1000G）
  - 变异优先级排序
- **依赖工具**: VEP, ANNOVAR, SnpEff

---

## 2. GWAS to Function (TWAS)

- **Skill ID**: `gwas-to-function-twas`
- **适用场景**: 复杂疾病遗传机制解析、治疗靶点发现
- **主要功能**:
  - GWAS 汇总统计输入
  - 转录组全关联研究（TWAS）分析
  - 因果基因优先排序
  - 组织特异性分析
  - 精细定位（Fine-mapping）
  - 治疗靶点候选基因列表
- **依赖工具**: FUSION, PrediXcan, S-PrediXcan

---

## 3. Mendelian Randomization

- **Skill ID**: `mendelian-randomization-twosamplemr`
- **适用场景**: 暴露-结局因果关系研究、流行病学
- **主要功能**:
  - 两样本孟德尔随机化（2SMR）
  - 工具变量筛选（F 统计量、LD 剪枝）
  - 多种 MR 方法（IVW, MR-Egger, WM, PRESSO）
  - 水平多效性检验
  - 敏感性分析
  - 因果效应估计与可视化
- **依赖工具**: TwoSampleMR, MendelianRandomization, R

---

## 4. Polygenic Risk Score (PRS Catalog)

- **Skill ID**: `polygenic-risk-score-prs-catalog`
- **适用场景**: 疾病风险预测、精准医学
- **主要功能**:
  - PGS Catalog 预计算权重下载
  - 单个或多个性状 PRS 计算
  - 人群参考分布比较
  - 风险分层与百分位数计算
  - PRS 性能评估（AUC, R²）
  - 多性状 PRS 整合
- **依赖工具**: pgscatalog-utils, PLINK2, R

---

[← 返回主目录](../README.md)
