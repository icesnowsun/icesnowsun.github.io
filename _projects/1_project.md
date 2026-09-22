---
layout: page
title: Modeling rapid kidney decline in CKDu
description: Which statistical model you choose changes who counts as a rapid decliner.
img: assets/img/project_ckdu.jpg
importance: 1
category: work
related_publications: true
---

Chronic kidney disease of uncertain etiology (CKDu) affects agricultural
communities in Sri Lanka without the usual drivers of kidney disease —
diabetes and hypertension — to explain it. Identifying who is declining
rapidly is the first step toward understanding why, and it turns out to depend
uncomfortably on how you ask.

## The question

"Rapid decline" sounds like an observation. It is actually a modeling choice.
In a cohort of 292 Sri Lankan participants I compared three approaches to the
same eGFR trajectories:

- **Ordinary least squares** — a slope per participant, fit independently
- **Linear mixed-effects** — participant slopes shrunk toward the population mean
- **Latent class mixed-effects** — participants sorted into distinct trajectory groups

Each gives a defensible answer. They do not give the same answer, and the
disagreement is not random noise: the models differ systematically in which
participants they flag, because they make different assumptions about whether
decline is a continuum or a set of types.

## Approach

Analyses were run pooled and stratified by sex, in R. Beyond the headline
comparison, two things needed care:

- **Censoring.** Participants enter and leave observation at different points,
  and the shape of that censoring interacts with slope estimation in ways that
  can manufacture apparent rapid decline.
- **Classification disagreement.** Rather than picking a winner, the useful
  output was characterizing *where* the methods diverge and what kind of
  participant falls into the gap.

I planned and validated the analyses jointly with a faculty mentor and wrote
the first-author poster {% cite yu2024rapiddecline %}, presented at the Joint
Statistical Meetings in 2024 and at the Stanford SRP Poster Symposium.

## Related work in this cohort

The same Sri Lankan cohort supports work on natural history and risk factors
{% cite hewavitharana2023ckdu %}, and a case-control study of drinking water and
agricultural exposures among women in endemic and non-endemic regions
{% cite contreras2026water %}.

## What I take from it

A single reported definition of rapid decline hides a decision that changes the
answer. Reporting the sensitivity of a finding to model class is cheap, and in
this setting it is more informative than the point estimate.
