---
layout: page
title: Measuring who a cohort actually represents
description: A generalizability score for comparing a study sample against the population it claims to describe.
img: assets/img/project_representativeness.jpg
importance: 2
category: work
related_publications: true
---

A research cohort recruited to study an underserved population can match that
population on paper and still miss badly in the places that matter. Aggregate
summaries are what hide this: a sample can look demographically close in the
margins while being wrong in every joint category.

## The question

RADx-UP was designed to reach communities underrepresented in COVID-19
research. Did it? Answering that requires more than comparing a few marginal
percentages against the census.

## Approach

I computed demographic representativeness scores comparing the RADx-UP cohort
against 2020 U.S. Census data, and programmed the comparisons so that gaps
obscured by aggregate reporting became visible — and, importantly, *visualizable*.
A score is only useful if someone can see where it comes from.

This became the first-author poster {% cite yu2025representativeness %} at the
Joint Statistical Meetings in 2025. After feedback there, I retitled and
re-presented it at the Stanford SRP Poster Symposium as *Generalizability Score
to Assess Sample Representativeness: Computation and Visualization*, shifting
emphasis from the RADx-UP finding to the reusable method.

## Why it generalizes

The construct is not specific to RADx-UP or to COVID-19. Any study that claims
to speak for a population invites the same question, and most answer it with a
table of marginal distributions. A score plus a visualization makes the gap
legible to the people running the study, not just to the statistician.

## Related infrastructure

The same trial supported reusable data workflows and R/SAS functions I built for
baseline tables, standardized differences, and missing-data summaries — the
unglamorous layer that makes this kind of analysis repeatable rather than a
one-off.
