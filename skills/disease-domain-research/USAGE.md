> 原作者：NanaTang | NanaTang Research Skills v1.0.0 | Copyright (c) 2026 NanaTang
> 允许内部工作使用；禁止未经授权转卖或收费包装 skill 及改写版本。分享时保留署名与许可，修改版本标记修改。详见随包 LICENSE。

# Disease Domain Research 使用指南

`disease-domain-research` 用来把一个疾病领域整理成结构化、可复核的研究结果。它支持从疾病认知开始，逐步扩展到治疗、市场、管线和产品机会。

## 最简单的用法

直接说明疾病、地区、研究阶段和交付格式：

```text
Use $disease-domain-research to complete Phase 1 for primary Sjögren disease in China and output a standalone HTML file.
```

如果不写阶段，Skill 会根据任务内容选择最小适用阶段，并在结果中说明范围。

## 阶段选择

| 阶段 | 适合回答的问题 | 典型产出 |
|---|---|---|
| Phase 1 | 这是什么病？有多少患者？如何确诊？患者如何分类？ | 疾病 Primer、机制图、患者旅程、诊断决策树、术语表 |
| Phase 2 | 怎么治疗？不同严重程度如何管理？还有什么未满足需求？ | 治疗路径、标准治疗表、疗效和安全性对比 |
| Phase 3 | 患病、确诊、治疗患者分别有多少？市场规模多大？ | 患者漏斗、患病/确诊/治疗/轻中重分层表、可及性分析 |
| Phase 4 | 有哪些在研产品？目标人群是什么？机会在哪里？ | 管线表、临床试验对比、产品机会分析 |
| Integrated DR | 希望一次完成完整疾病领域研究 | Phase 1–4 合并报告 |

## 推荐请求写法

### 只做疾病认知

```text
Use $disease-domain-research for Phase 1 on systemic lupus erythematosus, China-led with global context. The reader has no medical background. Output a beginner-friendly HTML report with sources.
```

### 重点做患者数据

```text
Use $disease-domain-research for Phase 3 on primary Sjögren disease in China. I need prevalence, epidemiologic patients, diagnosed patients, treated patients, and mild/moderate/severe patient counts in a table. For every number include definition, denominator, evidence type, source, and a verification link. Do not invent national rates.
```

### 研究某个产品的人群

```text
Use $disease-domain-research for Phase 4 on disease X. Compare the broad disease population with the target product's trial population, including disease background, biomarker, severity/activity, prior treatment, exclusion criteria, and estimated funnel size.
```

### 一次完成完整 DR

```text
Use $disease-domain-research for an Integrated DR on disease X in China. Start with a beginner-friendly disease primer, then add treatment, market/access, pipeline, and product opportunities. Output a standalone HTML file and a concise executive summary.
```

## 可以额外指定的要求

- **地区：** 中国为主、全球对照、某省/某城市或多个国家比较。
- **读者：** 零基础读者、咨询顾问、医学团队、市场准入、投资人或研发团队。
- **截止时间：** 例如“截至 2026 年 8 月”。
- **输出：** standalone HTML、Markdown、Excel-ready 表格、PPT 结构或简短 memo。
- **证据偏好：** 国家级指南、专家共识、PubMed 文献、ClinicalTrials.gov、监管文件或真实世界研究。
- **产品边界：** 指定药物、靶点、机制、试验编号或目标患者条件。

## 结果中的数字如何理解

Skill 会区分：

- 直接观测值；
- 区域或医院队列数据；
- 模型估算；
- 按患病率机械外推的量级；
- 基于假设的情景测算；
- 尚未找到公开全国统计的数据。

因此，结果可能明确写出“未找到全国公开确诊人数或治疗人数”，而不是用患病人数替代。这是为了避免把潜在患者池、确诊患者、治疗患者和产品可及患者混为一谈。

## 使用后的复核

重点检查三件事：

1. 每个数字的分母、地区、年份和疾病定义是否一致。
2. 来源链接是否能回到原始指南、论文、注册平台或监管文件。
3. 轻/中/重分层是否来自真实分布数据，而不是把单个医院队列直接外推到全国。

如需继续深化，可以在上一份结果基础上继续提出：

```text
继续 Phase 3，只补充中国确诊率、治疗率和严重程度分层；保留原有来源，并把新增数据标记出来。
```
