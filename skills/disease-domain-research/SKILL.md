---
name: disease-domain-research
description: Research and synthesize a disease domain in configurable phases, from a beginner-friendly disease primer through treatment, epidemiology, market/access, pipeline, and product-opportunity analysis. Use when Codex needs a China-led or global disease landscape, patient journey, diagnosis pathway, patient segmentation, treatment landscape, patient counts, clinical-trial pipeline, or evidence-backed HTML/table deliverable. Activate one or more phases explicitly (for example “Phase 1 disease primer”, “Phase 3 market”, or “full disease domain DR”); preserve definitions, denominators, source links, and uncertainty for every quantitative claim.
---

> 原作者：NanaTang | NanaTang Research Skills v1.0.0 | Copyright (c) 2026 NanaTang
> 允许内部工作使用；禁止未经授权转卖或收费包装 skill 及改写版本。分享时保留署名与许可，修改版本标记修改。详见随包 LICENSE。

# Disease Domain Research

## Purpose

Build an evidence-backed disease-domain deliverable that a reader with no prior knowledge can follow. Use a single research architecture with phase switches so the same method works for different diseases, geographies, audiences, and output formats.

## Phase Router

Parse the request before searching. Normalize:

- **Disease boundary:** disease name, synonyms, primary/secondary forms, legacy terminology, and whether a product-specific subgroup must be nested inside the broader disease.
- **Geography:** default to China-led when China is mentioned; separate China evidence from global context.
- **Population:** general population, diagnosed patients, treated patients, trial-eligible patients, or a payer/market population.
- **Time point:** current cut-off date and whether historical trend is needed.
- **Output:** standalone HTML, markdown/table, slide-ready outline, or another format.
- **Phase:** use the smallest set requested. If unspecified, start with Phase 1 and state the selected scope.

Available phases:

1. **Disease primer:** definition, mechanism, China/global epidemiology, patient journey, diagnostic decision tree, post-diagnosis classification, terms.
2. **Treatment and clinical management:** treatment goals, standard of care, severity/organ-based pathways, response endpoints, unmet needs.
3. **Market and access:** patient funnel, diagnosed/treated/managed populations, diagnosis and treatment rates, care settings, reimbursement and access.
4. **Pipeline and product opportunities:** approved and investigational products, mechanism, trial eligibility, endpoints, differentiation, white spaces.
5. **Integrated DR:** run Phases 1–4, then reconcile one common population funnel and source register.

Read only the reference file(s) needed for the selected phase:

- Phase 1: `references/phase-1-primer.md`
- Phase 2: `references/phase-2-treatment.md`
- Phase 3: `references/phase-3-market.md`
- Phase 4: `references/phase-4-pipeline.md`
- Any phase: `references/evidence-and-delivery.md`

## Non-negotiable Research Rules

1. **Conclusion first:** open each section with a one-sentence answer, then show the reasoning, supporting facts, caveats, and sources.
2. **Separate population layers:** never equate epidemiologic prevalence with diagnosed patients, treated patients, adequately managed patients, or product-eligible patients.
3. **Label evidence type:** mark every number as directly observed, modelled/estimated, mechanically extrapolated, or not publicly quantified.
4. **Show denominator and date:** state the numerator, denominator, geography, cohort, diagnostic definition, study year, and publication/access date whenever available.
5. **Prefer authoritative sources:** national clinical guidelines and consensus statements; government/registry statistics; systematic reviews and meta-analyses; large peer-reviewed cohorts; clinical-trial registries and regulatory documents. Use secondary market reports only when the methodology and denominator are visible.
6. **Do not manufacture missing rates:** if no national diagnosis or treatment rate exists, say so. A scenario estimate must be labelled as a scenario and must show the formula and assumptions.
7. **Reconcile conflicts:** explain differences caused by case definition, age range, region, period, ascertainment, assay, or severity threshold instead of averaging incompatible studies.
8. **Make clinical diagnosis distinct from research classification:** a score or trial criterion is not automatically the sole diagnostic algorithm.
9. **Explain terms on first use:** use `中文名称（English full name, abbreviation）+ one plain-language sentence`; subsequent uses may use an `<abbr title>` tooltip that includes a Chinese explanation.
10. **Keep products nested in disease context:** state which disease-background, biomarker/mechanism, severity/activity, prior-treatment, and safety filters define the target subgroup. Do not imply a trial subgroup is the whole disease.

## Source Retrieval And Citation

Use the life-science research router for broad questions, then the narrowest available source skill for retrieval (for example NCBI Entrez/PubMed for literature, ClinicalTrials.gov for trials, and official guideline pages for diagnosis). Record a stable URL for every source used. For PubMed, link to the article page rather than displaying an unlinked PMID. For Chinese sources, prefer the issuing society, journal, government, or registry page and preserve the original Chinese title.

Maintain a source register with: `source_id`, citation, source type, population/setting, year, key value, limitations, and verification link. Cite claims locally and repeat the full source register at the end of the deliverable.

## Quantitative Population Funnel

Use this common ladder in every disease landscape when relevant:

`total population → epidemiologic disease population → clinically recognized/diagnosed → receiving any treatment → receiving guideline-concordant management → eligible for a named product/trial`.

For each transition, report the observed value if available; otherwise write `未找到全国公开统计` and provide a bounded scenario only if assumptions are defensible. Never multiply several uncertain percentages without showing uncertainty propagation.

## Default Deliverable Structure

For a beginner-facing HTML report, use:

1. Executive summary with 3–5 conclusions.
2. What the disease is and how it works.
3. China patient scale and comparison with familiar diseases where valid.
4. Patient journey and diagnostic decision tree.
5. Post-diagnosis classification and how it changes management/outcomes.
6. Product-relevant subgroup funnel, if requested.
7. Searchable terms with full name, meaning, and first-use tooltip explanations.
8. Sources and evidence limitations.

For treatment/market/pipeline phases, append the corresponding modules without disrupting the primer storyline. Use tables for exact mappings and decision trees for sequential clinical pathways.

## Quality Check Before Delivery

- Every requested data category has a row or an explicit “not publicly quantified” entry.
- Every number has a definition, denominator, time/geography, evidence type, and source link.
- China and global estimates are not mixed in one total.
- Severity/activity categories use the source instrument’s actual thresholds; do not infer patient counts from a threshold without a distribution dataset.
- Diagnostic branches have an entry symptom, test purpose, result interpretation, next step, and endpoint; no single negative test is described as universally excluding disease.
- First-use abbreviations are explained in body text and tooltip text includes Chinese.
- HTML links, anchors, responsive layout, search/filter controls, and print layout are tested.
