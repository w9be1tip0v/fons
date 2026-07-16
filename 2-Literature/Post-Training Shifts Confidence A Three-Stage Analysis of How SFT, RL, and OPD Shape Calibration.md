---
title: "Post-Training Shifts Confidence: A Three-Stage Analysis of How SFT, RL, and OPD Shape Pre-, Intra-, and Post-CoT Calibration"
source: "https://arxiv.org/html/2607.13753v1"
author: "Shuhao Li, Guodong Du, Anhao Zhao, Wanyu Lin, Tianyu Yuan, Xiaoyu Shen"
published: "2026-07-15"
created: 2026-07-16
description: "Three-stage confidence framework shows OPD best for pre-reasoning confidence, SFT for early stopping, and RL for aggregation; PosConf improves RL aggregation by 6.1 points over majority vote."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/reasoning
  - keyword/evaluation
  - keyword/post-training
---

# Post-Training Shifts Confidence: A Three-Stage Analysis of How SFT, RL, and OPD Shape Pre-, Intra-, and Post-CoT Calibration

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.13753v1)
- published:: 2026-07-15
- updated:: 2026-07-15
- arxiv_id:: 2607.13753v1
- pdf:: https://arxiv.org/pdf/2607.13753v1
- categories:: cs.CL

## Abstract / Summary
LLMs gain reasoning from SFT, RL, and on-policy distillation (OPD), yet post-training is usually judged only by final-answer accuracy. This work studies how these methods reshape confidence before, during, and after chain-of-thought (difficulty estimation, early termination, answer aggregation). OPD provides the most useful pre-reasoning confidence, SFT the strongest online signal for early stopping, and RL the most reliable trace-level signal for aggregation. Confidence reliability is position-dependent. PosConf uses confidence only from reliable relative-position intervals, improving RL aggregation by 6.1 points over majority voting and OPD early stopping by up to 4.3 points under tight budgets. Code: https://github.com/EIT-NLP/Post-Training-Calibration.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.13753v1)
- [PDF](https://arxiv.org/pdf/2607.13753v1)
- [Code](https://github.com/EIT-NLP/Post-Training-Calibration)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/reasoning #keyword/evaluation #keyword/post-training
