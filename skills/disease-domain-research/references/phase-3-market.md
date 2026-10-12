> 原作者：NanaTang | NanaTang Research Skills v1.0.0 | Copyright (c) 2026 NanaTang
> 允许内部工作使用；禁止未经授权转卖或收费包装 skill 及改写版本。分享时保留署名与许可，修改版本标记修改。详见随包 LICENSE。

# Phase 3: Market, Patient Funnel, And Access

Read this file only when the request includes patient numbers, diagnosis/treatment rates, market sizing, care delivery, reimbursement, or access.

## Core Patient Funnel

Use mutually distinguishable layers:

1. **Epidemiologic disease population:** people meeting the study's disease definition, including undiagnosed cases.
2. **Clinically diagnosed population:** people recorded or judged as diagnosed in a defined period/data system.
3. **Treated population:** diagnosed people receiving the explicitly defined treatment class within a defined period.
4. **Guideline-managed population:** people receiving the relevant testing, monitoring, or therapy standard.
5. **Severity/activity subgroup:** people meeting a named, validated threshold in a representative dataset.
6. **Product-addressable population:** people additionally meeting indication/trial, biomarker, prior-treatment, contraindication, and access criteria.

## Mandatory Data Table

Always return this table even when data are missing:

| Data classification | Operational definition | China data | Evidence status | Calculation/assumptions | Source | Verification link | Limitation |
|---|---|---:|---|---|---|---|---|
| Prevalence | | | | | | | |
| Epidemiologic patient count | | | | | | | |
| Diagnosed patient count | | | | | | | |
| Diagnosis rate | Diagnosed / epidemiologic population | | | | | | |
| Treated patient count | | | | | | | |
| Treatment rate | Treated / diagnosed or epidemiologic population; state denominator | | | | | | |
| Mild/low activity | Named source threshold | | | | | | |
| Moderate activity | Named source threshold | | | | | | |
| Severe/high activity | Named source threshold | | | | | | |

Use `未找到全国公开统计` rather than leaving cells blank.

## Evidence Status Labels

- **Direct national observation:** a national registry, claims database, surveillance system, or representative national survey measured the value.
- **Direct subnational/cohort observation:** a regional survey or defined clinical cohort measured the value.
- **Modelled estimate:** a published model estimated the value.
- **Mechanical extrapolation:** prevalence × population, calculated for scale only.
- **Scenario:** user/analyst assumptions applied transparently.
- **Not publicly quantified:** no defensible public number was found by the search cut-off.

Do not present the last four categories as observed market size.

## Calculation Rules

Show formulas and units:

```text
epidemiologic patients = prevalence × applicable population
diagnosed patients = epidemiologic patients × diagnosis rate
treated patients = diagnosed patients × treatment rate among diagnosed
severity subgroup = compatible diagnosed/treated population × representative severity share
product-eligible = severity subgroup × biomarker share × other eligibility share
```

Apply uncertainty as ranges. Do not use a severity distribution from a tertiary hospital cohort to split the entire national epidemiologic population without a strong warning and a sensitivity range.

When studies use different severity instruments, keep them in separate rows. “Mild/moderate/severe,” physician global assessment, activity index bands, organ involvement, and treatment intensity are not interchangeable.

## Source Search Order

Search government statistics, national registries, insurance/claims studies, national or multi-region epidemiologic studies, national guidelines, peer-reviewed real-world cohorts, and transparent market reports. Search both Chinese and English disease names plus terms for prevalence, incidence, diagnosis, treatment, claims, registry, severity, activity, burden, and real-world evidence.

## Market Interpretation

After the table, provide three conclusions:

1. what is directly known;
2. what can only be bounded;
3. which missing variable most changes the opportunity estimate and therefore deserves primary research or database access.

Recommend validation routes for important gaps, such as national claims, hospital EMR networks, prescription audits, physician/patient research, or expert elicitation. Do not claim those data exist unless verified.
