# NanaTang Healthcare Research Skills

**原作者：NanaTang · v1.0.0 · Copyright (c) 2026 NanaTang**

GitHub 作者：[NanaTang-AI](https://github.com/NanaTang-AI) · 原始仓库：[Healthcare Research Skills](https://github.com/NanaTang-AI/nana-Healthcare-Research-skills)

允许工作使用，禁止未经授权转卖或收费包装 skill 及改写版本。详见 [使用许可](LICENSE) 与 [署名说明](ATTRIBUTION.md)。本项目为附使用限制的源码分享。

## 当前提供的 Skill

| Skill | 用途 |
|---|---|
| [disease-domain-research](skills/disease-domain-research/SKILL.md) | 分阶段研究疾病基础、诊疗、患者漏斗与准入、研发管线；保留来源、分母和不确定性 |

当前版本仅包含疾病领域研究 skill。

## 安装

下载本仓库，将 `skills/disease-domain-research/` 完整文件夹复制到 Codex 用户 skills 目录：

- Windows：`%USERPROFILE%\.codex\skills\`
- macOS / Linux：`~/.codex/skills/`
- 若设置了 `CODEX_HOME`，使用其下的 `skills/` 目录。

重新启动 Codex 或开启新会话。其他支持 `SKILL.md` 的工具，请遵循其安装说明。保留引用文件、元数据和许可。

## 研究阶段

| 阶段 | 范围 |
|---|---|
| Phase 1 | 疾病基础、机制、流行病学、患者旅程、诊断与分型 |
| Phase 2 | 临床管理、治疗路径、疗效终点与未满足需求 |
| Phase 3 | 患者漏斗、诊断与治疗率、市场规模和准入 |
| Phase 4 | 已上市产品、研发管线、临床试验与产品机会 |
| Integrated DR | 整合 Phase 1–4，统一患者口径和来源登记 |

## 使用示例

```text
使用 $disease-domain-research，完成中国某疾病的 Phase 1。面向没有医学背景的读者，输出带来源的疾病入门 HTML 报告。
```

```text
使用 $disease-domain-research，完成中国某疾病的 Phase 3。分别列出流行病学、确诊和在治患者规模，注明分母、时间、证据类型和来源；没有可靠数据时明确标记缺失。
```

## 环境与输出

需要可检索与核验原始资料的联网工具。文献、临床试验和指南检索工具按所在环境使用；特定检索插件不是使用本 skill 的唯一方式。

可按请求输出独立 HTML、Markdown 表格、适合幻灯片的内容提纲等形式，不包含固定 Word 模板。更多示例见 [使用说明](skills/disease-domain-research/USAGE.md)。

提供本次研究目标、范围、时间点及输入材料。输出用于研究与信息整理，临床结论应核验原始证据。
