> 原作者：NanaTang | NanaTang Research Skills v1.0.0 | Copyright (c) 2026 NanaTang
> 允许内部工作使用；禁止未经授权转卖或收费包装 skill 及改写版本。分享时保留署名与许可，修改版本标记修改。详见随包 LICENSE。

# Evidence, Synthesis, And Delivery Standards

Read this file for any phase that produces a user-facing report, table, HTML file, or quantitative conclusion.

## Evidence Ledger

Capture findings before writing prose:

| Claim ID | Claim | Value/unit | Definition/denominator | Geography/period | Evidence type | Source ID | Link | Limitation |
|---|---|---|---|---|---|---|---|---|

One source can support multiple claims, but every material claim must point to at least one source. Preserve contradictory findings as separate rows until reconciled.

## Source Hierarchy

Use the highest applicable level, not the highest level in the abstract:

1. Government, regulator, national registry, official guideline/consensus.
2. Systematic review/meta-analysis or representative epidemiologic study.
3. Large multicenter cohort, claims study, or randomized trial.
4. Single-center cohort, case-control study, or cross-sectional survey.
5. Conference abstract, company release, or transparent secondary report.
6. Unverifiable summary, search snippet, or unattributed figure: discovery only; do not cite as final evidence.

For trial design/status, the registry may outrank a paper. For approved wording, the regulator label outranks a review.

## Evidence Language

Use wording proportional to evidence:

- direct observation: “the study observed/reported”;
- model: “the model estimated”;
- extrapolation: “mechanically applying X to Y implies”;
- scenario: “under the stated assumptions”;
- gap: “no national public estimate was identified by the search cut-off.”

Do not write “China has N patients” when N is a mechanical extrapolation.

## Storyline

Use the pyramid principle:

1. answer the question in one sentence;
2. give 2–4 reasons or implications;
3. show supporting facts and comparisons;
4. explain limitations and unresolved gaps;
5. provide sources beside the claim and in a full register.

Explain the purpose of a classification or scale before its categories. Introduce familiar reference diseases only when definitions, years, and denominators are comparable enough to communicate magnitude.

## Standalone HTML

When HTML is requested, deliver one UTF-8 file that opens locally without a server. Include:

- sticky but compact section navigation;
- executive-summary band;
- responsive tables with horizontal overflow;
- vertically readable decision trees on mobile;
- searchable glossary when terms exceed ten;
- local claim citations linked to a source register;
- `<abbr>` tooltips containing a short Chinese explanation plus the English full name;
- print styles that remove navigation and preserve source URLs where practical;
- a visible research cut-off date and medical/non-promotional disclaimer.

Avoid cards nested inside cards, decorative gradients, oversized hero text, and one-note color palettes. Keep all important content readable at 360 px width and avoid connector-line overlaps.

## Table Delivery

For every requested metric, include:

- data classification;
- operational definition;
- value and unit;
- population/denominator;
- geography and period;
- direct observation versus calculation;
- source title/organization;
- stable verification link;
- limitation.

If the user requests fewer columns, retain definition, evidence status, source, and verification link somewhere in the table or notes.

## Verification Checklist

1. Open every link or verify it resolves to the intended source.
2. Recalculate every derived figure independently from displayed assumptions.
3. Confirm study population, case definition, and severity thresholds against the original source.
4. Check no count silently switches denominator between epidemiologic, diagnosed, and treated populations.
5. Check all acronyms at first use and all tooltip mappings.
6. Check HTML anchors, glossary search, mobile wrapping, print layout, and UTF-8 integrity.
7. State what was not found and which search cut-off applies.
