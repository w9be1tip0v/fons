---
title: "teLLMe Why (Ain't Nothing but a Jam): Exploratory Causal Analysis of Urban Driving Data"
source: "https://arxiv.org/html/2607.15254v1"
author: "Qiwei Li, Jorge Ortiz"
published: "2026-07-16"
created: 2026-07-19
description: "Schema-aware LLM maps NL questions to causal queries over dashcam event tables; PC + bootstrap + DoWhy yield Causal Cards for urban traffic hypothesis generation (NeurIPS 2025 UrbanAI)."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/agents
  - keyword/ai
---

# teLLMe Why (Ain't Nothing but a Jam): Exploratory Causal Analysis of Urban Driving Data

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15254v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15254v1
- pdf:: https://arxiv.org/pdf/2607.15254v1
- categories:: cs.AI, cs.LG (NeurIPS 2025 Workshop on UrbanAI)

## Abstract / Summary
Traffic agencies have large video-derived observational datasets, making causal questions (e.g., rain → density) hard. teLLMe supports exploratory causal analysis of urban driving data: structured event tables from dashcam annotations, PC algorithm causal structure learning, bootstrap stability checks, and query-specific effect estimation via linear regression and DoWhy. A schema-aware LLM maps natural-language questions to structured causal queries (treatments, outcomes, subpopulations). Output is a Causal Card (effect estimates, adjustment sets, DAG support, assumptions) plus a short NL explanation. BDD-derived case studies surface plausible weather/peak-hour/density relationships while making uncertainty and modeling choices explicit—aimed at hypothesis generation, not definitive causal claims.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15254v1)
- [PDF](https://arxiv.org/pdf/2607.15254v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/agents #keyword/ai
