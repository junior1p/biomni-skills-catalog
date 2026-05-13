# 💊 药物发现与临床技能

本目录收录 Biomni 平台中与药物靶点发现、临床试验分析和生物标志物研究相关的技能。

---

## 1. Open Targets Platform

- **Skill ID**: `open-targets`
- **适用场景**: 靶点-疾病关联分析、药物靶点优先排序
- **主要功能**:
  - 靶点注释（可成药性、必需性、表达、约束）
  - 疾病注释（本体、已知药物、关联靶点）
  - 药物/化合物信息（作用机制、适应症、临床阶段）
  - 靶点-疾病关联评分（20+ 数据源）
  - 变异与 GWAS 数据（L2G 预测、共定位）
  - 名称 → ID 解析
- **API**: GraphQL (https://api.platform.opentargets.org/api/v4/graphql)
- **数据许可**: CC0 1.0

---

## 2. scRNA Disease Drug Discovery

- **Skill ID**: `scrna-disease-drug-discovery`
- **适用场景**: 疾病机制研究、多组学靶点发现
- **主要功能**:
  - 端到端单细胞 RNA-seq 疾病分析
  - 疾病细胞类型识别与特征分析
  - 遗传证据整合（GWAS、eQTL）
  - 多组学药物靶点优先排序
  - 靶点可成药性评估
  - 候选靶点报告生成
- **依赖工具**: Scanpy, Open Targets API, Python

---

## 3. ClinicalTrials Landscape

- **Skill ID**: `clinicaltrials-landscape`
- **适用场景**: 竞争格局分析、研发策略制定
- **主要功能**:
  - ClinicalTrials.gov API v2 查询
  - 按疾病领域、机制、阶段、申办方筛选
  - 临床试验全景图绘制
  - 试验状态与结果追踪
  - 竞争格局可视化
  - 数据导出（CSV/Excel）
- **数据来源**: ClinicalTrials.gov

---

## 4. Literature Preclinical

- **Skill ID**: `literature-preclinical`
- **适用场景**: 靶点验证、临床前证据综合
- **主要功能**:
  - 靶点-疾病临床前文献搜索
  - 体内实验详情提取（动物模型、给药方案、结果）
  - 体外实验详情提取（细胞系、浓度、终点）
  - 结构化证据汇总
  - 证据强度评估
- **数据来源**: PubMed, bioRxiv, EuropePMC

---

## 5. LASSO Biomarker Panel

- **Skill ID**: `lasso-biomarker-panel`
- **适用场景**: 诊断标志物开发、预后模型构建
- **主要功能**:
  - LASSO 正则化特征选择
  - 嵌套交叉验证（避免过拟合）
  - 稳定性选择（Stability Selection）
  - 独立队列验证
  - 最小生物标志物面板输出
  - 模型性能评估（AUC, 校准曲线）
- **依赖工具**: glmnet, caret, R

---

## 6. Survival Analysis Clinical

- **Skill ID**: `survival-analysis-clinical`
- **适用场景**: 临床预后研究、生存分析
- **主要功能**:
  - Kaplan-Meier 生存曲线估计
  - Log-rank 检验
  - Cox 比例风险回归
  - 多变量生存分析
  - 风险分层（高/低风险组）
  - 时间依赖 ROC 分析
- **依赖工具**: survival, survminer, R

---

[← 返回主目录](../README.md)
