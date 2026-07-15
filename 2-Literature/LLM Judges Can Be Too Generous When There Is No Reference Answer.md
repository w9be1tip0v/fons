---
title: "LLM Judges Can Be Too Generous When There Is No Reference Answer"
source: "https://arxiv.org/html/2607.12885v1"
author: "Chalamalasetti Kranti, Sowmya Vajjala"
published: "2026-07-14"
created: 2026-07-16
description: "Calibration and sensitivity study of LLM-as-judge setups without reference answers: judges over-credit incorrect answers, and adding reference text can flip correct/incorrect decisions by up to 85%."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/ai
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
  - keyword/research-paper
---

# LLM Judges Can Be Too Generous When There Is No Reference Answer

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.12885v1)
- published:: 2026-07-14
- updated:: 2026-07-14
- arxiv_id:: 2607.12885v1
- pdf:: https://arxiv.org/pdf/2607.12885v1
- categories:: cs.CL

## Abstract / Summary
LLM judges are increasingly being used to evaluate open-ended model responses, often in no-reference settings where a ground-truth answer is unavailable. However, can they reliably assess in such evaluation setups? We explore this question in this paper through a two stage pipeline with a) calibration experiments that assess the judge model's knowledge of the task it is evaluating, and b) sensitivity experiments that assess how the judge model's performance is impacted by the presence and positioning of the reference answer in the prompt. Across experiments covering three languages, we show that the judge models we evaluated tend to over-credit incorrect answers in the absence of a reference answer, and adding reference answer information to the prompt flips the judge model's correct/incorrect decisions by as much as 85% in some experimental settings. Comparison with a subset of human annotations shows that these reference-driven changes generally align with human judgments. Our results emphasize the need for calibrating the LLM judges with a sample with reference-aware evaluation before using them in reference-free setups reliably, and our methodology provides a blueprint for researchers and practitioners in doing such calibration of LLM judges for other tasks.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.12885)
- [PDF](https://arxiv.org/pdf/2607.12885v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/ai #keyword/evaluation #keyword/benchmark #keyword/machine-learning #keyword/research-paper
