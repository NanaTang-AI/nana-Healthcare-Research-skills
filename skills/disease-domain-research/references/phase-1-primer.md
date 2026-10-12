> 原作者：NanaTang | NanaTang Research Skills v1.0.0 | Copyright (c) 2026 NanaTang
> 允许内部工作使用；禁止未经授权转卖或收费包装 skill 及改写版本。分享时保留署名与许可，修改版本标记修改。详见随包 LICENSE。

# Phase 1: Disease Primer

Read this file only when the request includes disease understanding, epidemiology, diagnosis, patient journey, classification, or terminology.

## Research Questions

Answer in this order for a beginner:

1. What is the disease, and what is outside its boundary?
2. What biological sequence causes symptoms and organ damage?
3. How many people may have it in the requested geography?
4. How does a patient move from first symptoms to clinical suspicion and diagnosis?
5. After diagnosis, which classification axes change testing, treatment, prognosis, or trial eligibility?
6. Where does a named product population sit inside the broad disease?

## Disease Boundary

Normalize current and legacy names. Explain primary/secondary, organ-limited/systemic, acute/chronic, adult/pediatric, inherited/acquired, or other disease-specific distinctions before using them. Treat classification axes independently until evidence links them.

Create a boundary table:

| Boundary | Included | Excluded or separate | Why it matters |
|---|---|---|---|
| Broad disease | | | Epidemiology |
| Clinical diagnosis | | | Care pathway |
| Research classification | | | Study comparability |
| Product/trial subgroup | | | Opportunity sizing |

## Mechanism Story

Translate mechanism into a causal chain:

`predisposition/exposure → initiating event → cell/pathway dysregulation → tissue dysfunction → symptoms → organ damage/complications`.

For each link, distinguish established biology from a hypothesis. Explain biomarkers as diagnostic, prognostic, predictive, pharmacodynamic, or merely associated. When a product targets one node, say whether the trial actually requires that biomarker; do not invent a companion-diagnostic subtype.

## Epidemiology

Search separately for prevalence, incidence, age/sex distribution, regional variation, time trend, diagnostic delay, and underdiagnosis. Prefer national or multi-region data; use single-city or hospital cohorts only with explicit caveats.

Use a table with these columns:

| Data category | Definition | Geography/period | Observed data | Population equivalent | Evidence type | Source | Verification link | Caveat |
|---|---|---|---:|---:|---|---|---|---|

When converting prevalence to people, show the formula and population base. Call it a mechanical extrapolation, not a national patient count.

## Patient Journey And Diagnosis

Use national guidelines and national-level expert consensus as the backbone. Supplement with international classification criteria only to explain objective thresholds.

Construct a decision tree with these stages:

1. **Entry symptoms/complaints:** common symptoms, duration, red flags, and atypical organ presentations.
2. **First care setting:** likely departments and reasons for fragmented presentation.
3. **Clinical suspicion:** the symptom combinations or lab/organ signals that trigger referral.
4. **Alternative causes:** common mimics, medication effects, exclusion criteria, and test-interfering factors.
5. **First-line tests:** purpose, positive/negative interpretation, department, patient burden, and typical availability.
6. **Objective/specialist tests:** thresholds, quality requirements, limitations, and availability by hospital level.
7. **Result branches:** what a positive or negative result changes; avoid “one negative test excludes disease” unless the guideline explicitly says so.
8. **Final clinical judgment:** distinguish clinical diagnosis, research classification, severity/activity assessment, and organ-risk workup.

Every branch must contain an entry, test or decision, interpretation, next step, and endpoint.

## Post-diagnosis Classification

Explain why classification matters before listing categories. Select disease-relevant axes such as:

- disease background or etiology;
- affected organs/phenotype;
- severity or activity;
- patient-reported symptom burden;
- biomarker/immune/molecular phenotype;
- structural damage or remaining organ reserve;
- prognosis/risk;
- treatment history and refractoriness.

For every scale, provide the full name, assessor (doctor/patient/lab), domains, range, thresholds, and clinical consequence. Show that two axes may be discordant with short patient examples.

Do not convert severity percentages into national counts unless a compatible population denominator and a representative severity distribution are both available.

## Terms

At first use, write `中文名称（English full name, abbreviation）` and one plain-language explanation. In HTML, later uses may be:

```html
<abbr title="中文简短解释；英文全称：English Full Name">ABC</abbr>
```

Also provide a searchable glossary with abbreviation, English full name, Chinese name, what it measures/means, and why it matters.
