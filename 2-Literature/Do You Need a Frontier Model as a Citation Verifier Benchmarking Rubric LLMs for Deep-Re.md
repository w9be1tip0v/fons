---
title: "Do You Need a Frontier Model as a Citation Verifier? Benchmarking Rubric LLMs for Deep-Research Source Attribution"
source: "https://arxiv.org/html/2607.08700v1"
author: "Ethan Leung, Elias Lumer, Corey Feld, Austin Huber, Vamse Kumar Subbiah, Kevin Paul"
published: "2026-07-09"
created: 2026-07-11
description: "Reinforcement learning increasingly relies on an LLM judge to score each rubric criterion, and that judge acts as the reward model during training. Before such a signal can be trusted, we need to know how capable the judge must be and how biased it is. We study this calibration question for citation quality in deep-research systems, where a search-grounded LLM must support each claim it writes with a cited source. C…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
---

# Do You Need a Frontier Model as a Citation Verifier? Benchmarking Rubric LLMs for Deep-Research Source Attribution

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.08700v1)
- published:: 2026-07-09
- updated:: 2026-07-09
- arxiv_id:: 2607.08700v1
- pdf:: https://arxiv.org/pdf/2607.08700v1
- categories:: cs.CL

## Abstract / Summary
Reinforcement learning increasingly relies on an LLM judge to score each rubric criterion, and that judge acts as the reward model during training. Before such a signal can be trusted, we need to know how capable the judge must be and how biased it is. We study this calibration question for citation quality in deep-research systems, where a search-grounded LLM must support each claim it writes with a cited source. Citation quality is a structured rubric task in which each attribution-citation pair is judged along two dimensions that require an LLM, source relevance and factual support. On an adversarial long-form benchmark, we score 8 off-the-shelf LLM judges from 3 model families against gold labels over 1,248 rubric decisions, all of which were human-reviewed and 378 of which were hard cases adjudicated from judge disagreements. Cheaper judges remain competitive across both dimensions, with GPT-5-mini attaining the strongest source-relevance pass-class F1 at 0.908 ($κ$=0.636), while on factual support the judges are statistically indistinguishable (overlapping confidence intervals), so no single model dominates. At comparable F1, the judges still differ substantially in pass-rate drift, false positive rate, and false negative rate. Scalar F1 obscures this directional bias, yet it is exactly what a downstream reinforcement learning loop would reinforce. Calibrating the judge is therefore a prerequisite for using citation rubrics as reward signals, and our results show that this calibration does not require the most expensive available model.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.08700v1)
- [PDF](https://arxiv.org/pdf/2607.08700v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/evaluation #keyword/benchmark #keyword/machine-learning
