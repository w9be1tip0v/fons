---
title: "The Illusion of Robustness: Aggregate Accuracy Hides Prediction Flips under Task-Irrelevant Context"
source: "https://arxiv.org/html/2607.12963v1"
author: "Yanzhe Zhang, Sanmi Koyejo, Diyi Yang"
published: "2026-07-14"
created: 2026-07-16
description: "Shows that aggregate LLM accuracy under task-irrelevant context can look stable while per-example predictions flip substantially, even from meaningless pseudo-words, motivating per-example reliability evaluation."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/ai
  - keyword/evaluation
  - keyword/safety
  - keyword/machine-learning
  - keyword/research-paper
---

# The Illusion of Robustness: Aggregate Accuracy Hides Prediction Flips under Task-Irrelevant Context

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.12963v1)
- published:: 2026-07-14
- updated:: 2026-07-14
- arxiv_id:: 2607.12963v1
- pdf:: https://arxiv.org/pdf/2607.12963v1
- categories:: cs.CL

## Abstract / Summary
As large language models (LLMs) grow more capable, they are increasingly deployed in context-rich settings where task inputs are often accompanied by long, partially irrelevant context. In a controlled setting, we find that state-of-the-art models often appear robust to task-irrelevant context at the aggregate level: prepending it to benchmark questions causes little change in overall accuracy. This aggregate stability, however, masks significant per-example instability. Even semantically meaningless pseudo-words, formed by randomly combining characters, can markedly shift model predictions on a small fraction of examples, degrading performance on some while improving it on others. This two-sided effect holds consistently across a wide range of models and datasets, yet the affected examples are largely model-specific. We further show that this instability is modulated by context type, context length, test-time compute, and model development stage. Together, our findings reveal context-induced tail risks concealed by aggregate accuracy, motivating per-example reliability evaluation of language models.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.12963)
- [PDF](https://arxiv.org/pdf/2607.12963v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/ai #keyword/evaluation #keyword/safety #keyword/machine-learning #keyword/research-paper
