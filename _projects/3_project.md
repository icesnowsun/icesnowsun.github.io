---
layout: page
title: Dialysis care — surveillance, vaccination, and access
description: Trials and national studies on COVID-19 surveillance in dialysis facilities and on where dialysis care is disappearing.
img: assets/img/project_dialysis.jpg
importance: 3
category: work
related_publications: true
---

People receiving in-center hemodialysis attend a clinical facility three times a
week, every week. During the pandemic that made them both unusually exposed and
unusually observable — a population where surveillance was feasible precisely
because they could not stay home.

## Surveillance and vaccination

A pilot established that SARS-CoV-2 screening during routine hemodialysis was
feasible and acceptable to patients {% cite anand2023feasibility %}. That scaled
into a nationwide cluster randomized trial across 62 US Renal Care dialysis
centers {% cite montezrath2024acceptance %}, conducted under the NIH
[RADx-UP](https://radx-up.org/about/) initiative, whose aim is improving access
to COVID-19 testing in underserved communities.

My role on the trial was the weekly data pipeline — cleaning and processing
testing data, building the tables and figures clinicians actually read, handling
missing data by multiple imputation with chained equations, and using
generalized estimating equations to account for clustering by facility.

Separately, we asked whether wastewater could substitute for case reporting once
at-home testing made official case counts unreliable
{% cite varkila2023wastewater %}. Using public data from more than 250 U.S.
counties, we found that *wastewater percentile* — a county’s current
concentration relative to its own historic peak — predicted high case rates with
an AUC of 0.95 in early 2022, with a threshold around the 51st percentile
maximizing sensitivity and specificity. Performance degraded in later quarters,
which is itself informative: as reporting decayed, the wastewater signal and the
official counts diverged.

A preprint examines whether the *time of day* a patient receives a SARS-CoV-2
vaccination is associated with their antibody response
{% cite subramanian2025timeofday %} — a circadian question that the fixed,
repeating schedule of dialysis care happens to make answerable.

## Access

The other half of this thread is structural rather than clinical: a serial
cross-sectional study of dialysis facility closures across the U.S. from 2018 to
2024 {% cite varkila2026closures %}. Closures are not distributed evenly, and
for a treatment that requires physically attending a facility three times a
week, distance is not an inconvenience — it is a determinant of whether
treatment happens.

Related work looks at the gap between how patients understand their kidney
disease and their clinical diagnosis in California's Central Valley
{% cite contreras2026cjasn %}, and at kidney function differences across rural
and urban communities in India {% cite subramanian2025india %}.

## My role

Across these studies I contributed statistical programming and analysis, working
with the nephrology and epidemiology teams at Stanford who led the clinical
design.
