# Disease Domain Research · 疾病领域研究

**An evidence-focused AI skill for understanding diseases, mapping treatment pathways, sizing patient populations, and assessing pipelines.**
**一个以证据为基础的 AI 研究 skill，帮助理解疾病、梳理诊疗路径、估算患者规模并分析研发管线。**

Author / 作者：**NanaTang** · Skill：`disease-domain-research` · Version / 版本：**1.0.0**

[中文说明](#中文说明) · [English](#english) · [License / 使用许可](LICENSE) · [Source / 原始仓库](https://github.com/NanaTang-AI/nana-Healthcare-Research-skills)

## 中文说明

### 简介

Disease Domain Research 将疾病研究组织为可按需调用的模块：从疾病机制、流行病学和患者旅程，到诊疗格局、患者漏斗、市场准入与研发管线。可用于中国或全球疾病领域研究，并根据读者背景输出易理解的 HTML 报告、Markdown 表格或适合幻灯片的内容提纲。

研究要求包括：明确患者定义与数据分母，区分观察数据、估算和假设，保留可核验的来源，并如实标记信息缺口。它提供研究工作流，不自带商业数据库，也不保证每个问题都有公开数据。

### 适合谁使用

医疗咨询、医药行业研究、商业策略、市场准入、产品规划，以及需要快速建立疾病领域认知的研究者。

### 研究模块

| 模块 | 核心内容 |
|---|---|
| Phase 1：疾病基础 | 定义与机制、流行病学、患者旅程、诊断路径、诊后分类与术语 |
| Phase 2：临床管理 | 治疗目标、标准治疗、患者分层与治疗路径、疗效终点、未满足需求 |
| Phase 3：市场与准入 | 流行病学／确诊／在治患者漏斗、诊断与治疗率、照护场景、支付与准入 |
| Phase 4：管线与产品机会 | 已上市与在研产品、机制、试验人群、终点、差异化及证据缺口 |
| Integrated DR：整合研究 | 整合 Phase 1–4，并统一患者口径、推算假设与来源登记 |

可选择一个或多个模块；未指定阶段时，从 Phase 1 开始。研究地区、疾病边界、截止日期和输出形式可按任务设置。

### 研究原则

- **不同患者人群分开统计**：患病、确诊、在治、规范管理和产品适用人群不能互相替代。
- **每个关键数字保留口径**：定义、分母、地区、时间和证据类型应清楚可查。
- **缺失数据如实标记**：不虚构全国诊断率或治疗率；推算需要展示公式和假设。
- **优先核验原始证据**：指南、政府／登记数据、同行评审研究、试验注册和监管资料。
- **结论与证据相连**：先给出回答，再解释依据、局限和不确定性。

### 安装

1. 点击仓库的 **Code → Download ZIP**，下载并解压。
2. 将 `skills/disease-domain-research/` **整个文件夹**复制到 Codex 用户 skills 目录：

| 环境 | 目录 |
|---|---|
| Windows | `%USERPROFILE%\.codex\skills\` |
| macOS / Linux | `~/.codex/skills/` |
| 自定义 `CODEX_HOME` | `$CODEX_HOME/skills/` |

3. 重启 Codex 或开启新会话，使用 `$disease-domain-research` 调用。

请保留文件夹中的 `SKILL.md`、`references/`、`agents/` 和 `LICENSE`。其他支持 skill 的工具请遵循其安装说明，本仓库未验证全部工具的兼容性。

### 使用示例

**疾病入门**

```text
使用 $disease-domain-research，完成系统性红斑狼疮的 Phase 1。
以中国为主，补充全球背景；面向没有医学背景的读者。
输出独立 HTML 报告，说明机制、流行病学、患者旅程、诊断与分型，并保留来源链接。
```

**患者漏斗与市场研究**

```text
使用 $disease-domain-research，完成中国某疾病的 Phase 3。
分别列出流行病学、确诊和在治患者规模，注明定义、分母、时间、证据类型及来源。
推算展示公式与假设；没有可靠公开数据时明确标记缺失。输出 Markdown 表格。
```

提供疾病、地区、研究阶段、研究截止日期、目标读者和输出形式即可开始；有产品或患者亚组要求时，请一并说明。

### 工具与输出

需要能够检索并核验原始资料的联网环境。可使用 PubMed、ClinicalTrials.gov、官方指南及监管网站等资料来源；实际可用工具取决于运行环境，skill 不附带数据库账号或检索权限。

支持按请求生成独立 HTML、Markdown／表格和适合幻灯片的内容提纲，无需固定 Word 模板。完整示例见 [使用说明](skills/disease-domain-research/USAGE.md)。

研究结果需要复核，尤其是临床结论、产品状态和患者规模估算；本 skill 用于研究与信息整理，不替代临床决策。

## English

### Overview

Disease Domain Research organizes disease research into configurable modules, covering disease biology, epidemiology, patient journeys, treatment landscapes, patient funnels, market access, and clinical pipelines. It supports China-focused or global research and can produce accessible HTML reports, Markdown tables, or slide-ready content outlines.

The workflow emphasizes explicit population definitions and denominators, clear separation of observed data from estimates and assumptions, verifiable sources, and transparent data gaps. It supplies research instructions, not a proprietary database or a guarantee that public evidence exists for every question.

### Who it is for

Healthcare consultants, pharmaceutical researchers, commercial strategy and market-access teams, product planners, and researchers building familiarity with a disease area.

### Research modules

| Module | Coverage |
|---|---|
| Phase 1: Disease primer | Definition, biology, epidemiology, patient journey, diagnosis, classification, and terminology |
| Phase 2: Clinical management | Treatment goals, standard of care, patient segmentation, pathways, endpoints, and unmet needs |
| Phase 3: Market and access | Epidemiologic, diagnosed, and treated patient funnels; diagnosis and treatment rates; care settings; payment and access |
| Phase 4: Pipeline and product opportunities | Approved and investigational assets, mechanisms, trial populations, endpoints, differentiation, and evidence gaps |
| Integrated DR | Phases 1–4 with consistent population definitions, calculation assumptions, and a source register |

Select one or more modules. If no phase is specified, the skill starts with Phase 1. Geography, disease boundaries, research cut-off date, audience, and output format are configurable.

### Research principles

- **Separate population layers:** prevalence, diagnosis, treatment, guideline-concordant management, and product eligibility are distinct.
- **Make numbers interpretable:** preserve definitions, denominators, geography, dates, and evidence types.
- **Report missing data honestly:** do not invent national diagnosis or treatment rates; show formulas and assumptions for estimates.
- **Verify primary evidence:** prioritize guidelines, government and registry data, peer-reviewed studies, trial registries, and regulatory sources.
- **Connect conclusions to evidence:** lead with the answer, then explain its basis, limitations, and uncertainty.

### Installation

1. Select **Code → Download ZIP** on GitHub and extract the archive.
2. Copy the **entire** `skills/disease-domain-research/` folder into your Codex user skills directory:

| Environment | Directory |
|---|---|
| Windows | `%USERPROFILE%\.codex\skills\` |
| macOS / Linux | `~/.codex/skills/` |
| Custom `CODEX_HOME` | `$CODEX_HOME/skills/` |

3. Restart Codex or start a new session, then invoke `$disease-domain-research`.

Keep `SKILL.md`, `references/`, `agents/`, and `LICENSE` together. Follow the installation instructions of other skill-compatible tools; compatibility with every tool has not been verified.

### Example prompts

**Disease primer**

```text
Use $disease-domain-research for Phase 1 on systemic lupus erythematosus.
Focus on China with global context, for readers without a medical background.
Create a standalone HTML report covering biology, epidemiology, patient journey,
diagnosis, and classification, with source links.
```

**Patient funnel and market research**

```text
Use $disease-domain-research for Phase 3 on a disease in China.
Separate epidemiologic, diagnosed, and treated patient counts.
Include definitions, denominators, dates, evidence types, and sources.
Show formulas and assumptions for estimates, and explicitly flag unavailable
public data. Output Markdown tables.
```

Specify the disease, geography, phase, research cut-off date, audience, and output format. Add any product-specific or patient-subgroup requirements.

### Tools and outputs

An environment with access to search and verify primary sources is required. Sources may include PubMed, ClinicalTrials.gov, official guidelines, and regulatory websites. Available tools depend on the host environment; database accounts and access permissions are not included.

Outputs may include standalone HTML, Markdown tables, and slide-ready content outlines. No fixed Word template is required. See [additional usage examples](skills/disease-domain-research/USAGE.md).

Verify findings before use, especially clinical conclusions, product status, and population estimates. This skill supports research and information synthesis; it does not replace clinical decision-making.

## License · 使用许可

**允许 / Permitted:** 学习、个人或公司内部工作、内部修改，以及交付独立研究成果。
Learning, personal or organizational internal work, internal modifications, and delivery of independently produced research outputs.

**需另行授权 / Separate permission required:** 转卖或收费分发 skill 及实质性改写版本，或将其包装为收费课程、付费插件、订阅产品或对外托管 skill 服务。
Selling or distributing the skill or substantial adaptations for a fee, or packaging them in paid courses, plugins, subscription products, or hosted skill services.

免费分享材料时保留作者、来源与许可，修改版本注明修改。使用者独立成果不自动归作者所有，也无需在每份客户成果中展示 skill 作者署名。
When sharing materials for free, preserve attribution, source information, and the license, and identify modifications. Independently produced user outputs do not automatically belong to the skill author, and each client deliverable does not require skill-author branding.

完整条款以 [LICENSE](LICENSE) 为准。本项目为附限制的源码分享，不宣称采用标准开源许可。
The full [LICENSE](LICENSE) governs. This is source sharing under a custom restricted-use license, not a claim of standard open-source licensing.

**Copyright (c) 2026 NanaTang.**
[Author / 作者](https://github.com/NanaTang-AI) · [Attribution / 署名说明](ATTRIBUTION.md) · [Release checks / 发布检查](RELEASE_CHECK.md)
