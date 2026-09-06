---
title: "Landmark-Based Discrimination of Injury-Associated Athlete-Sessions from Minute-Resolution Multimodal Football Monitoring Data"
source: "https://arxiv.org/html/2609.03790v1"
author: "Evangelos Chatzidimitriou, Konstantinos Tserpes"
published: "2026-09-03"
created: 2026-09-07
description: "Athlete monitoring data may be recorded minute by minute throughout a match or training session, while injury information may only indicate whether the entire session was injury-associated. This creates a modelling problem: assigning the same session-level label to every minute would imply that injury status is known at each exact time, even though within-session injury onset is unknown. Our novelty is a fixed-landm…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/multimodal
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
---

# Landmark-Based Discrimination of Injury-Associated Athlete-Sessions from Minute-Resolution Multimodal Football Monitoring Data

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.03790v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.03790v1
- pdf:: https://arxiv.org/pdf/2609.03790v1
- categories:: cs.LG

## Abstract / Summary
Athlete monitoring data may be recorded minute by minute throughout a match or training session, while injury information may only indicate whether the entire session was injury-associated. This creates a modelling problem: assigning the same session-level label to every minute would imply that injury status is known at each exact time, even though within-session injury onset is unknown. Our novelty is a fixed-landmark, one-representation-per-athlete-session formulation that directly addresses this mismatch. Instead of labelling every minute, we construct one representation per athlete-session at each landmark using information observed up to that point. This keeps the target at the session level and avoids unsupported minute-level injury supervision. A landmark is a fixed time point within the same session, such as 10, 20, or 30 minutes. At each landmark, we assess whether the whole session is injury-associated or non-injury-associated and examine how discrimination changes as more within-session information becomes available. Using 2020 SoccerMon data, we analyse 3,743 athlete-sessions from 48 elite women's football athletes, including 22 injury-associated sessions from five athletes. We evaluate pre-session, cumulative, dynamic, and combined representations with athlete-disjoint validation, athlete-cluster bootstrap uncertainty, common-cohort sensitivity analysis, alternative negative-athlete fold allocations, equal-athlete weighting, and Logistic Regression, Random Forest, and XGBoost benchmarks. Primary CUM+DYN Logistic Regression yields ROC-AUC 0.367-0.607 and PR-AUC 0.0080-0.0150 across landmarks, with wide uncertainty. PRE-containing representations show higher point estimates at several landmarks but remain uncertain.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.03790v1)
- [PDF](https://arxiv.org/pdf/2609.03790v1)
- [Machine learning models for injury risk prediction in football players: A systematic review of predictors, performance, practical applications, and limitations](https://doi.org/10.1177/03000605261469442) (2026, citations: 1)
- [Time-to-Injury Forecasting in Elite Female Football: A DeepHit Survival Approach](https://arxiv.org/abs/2601.19479) (2026, citations: 2)
- [SoccerGuard: Investigating Injury Risk Factors for Professional Soccer Players with Machine Learning](https://arxiv.org/abs/2411.08901) (2024, citations: 3)
- [A large-scale multivariate soccer athlete health, performance, and position monitoring dataset](https://www.nature.com/articles/s41597-024-03386-x.pdf) (2024, citations: 13)
- [Analysis of peak locomotor demands in women’s football–the influence of different epoch lengths](https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0303759&type=printable) (2024, citations: 8)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/multimodal #keyword/evaluation #keyword/benchmark #keyword/machine-learning
