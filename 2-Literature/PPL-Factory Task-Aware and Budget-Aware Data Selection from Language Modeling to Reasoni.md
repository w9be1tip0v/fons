---
title: "PPL-Factory: Task-Aware and Budget-Aware Data Selection from Language Modeling to Reasoning"
source: "https://arxiv.org/html/2607.18199v1"
author: "Hang Zhang, Warren J. Gross"
published: "2026-07-20"
created: 2026-07-22
description: "Not all training samples contribute equally to large language model fine-tuning. Selecting informative training samples can reduce the computational cost while preserving downstream performance. Many existing data selection methods rely on indirect heuristics, such as data quality, diversity or reasoning trace length. However, the effectiveness of these fixed criteria is task-dependent and difficult to generalize ac…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/reasoning
  - keyword/machine-learning
  - keyword/research-paper
---

# PPL-Factory: Task-Aware and Budget-Aware Data Selection from Language Modeling to Reasoning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.18199v1)
- published:: 2026-07-20
- updated:: 2026-07-20
- arxiv_id:: 2607.18199v1
- pdf:: https://arxiv.org/pdf/2607.18199v1
- categories:: cs.CL, cs.LG

## Abstract / Summary
Not all training samples contribute equally to large language model fine-tuning. Selecting informative training samples can reduce the computational cost while preserving downstream performance. Many existing data selection methods rely on indirect heuristics, such as data quality, diversity or reasoning trace length. However, the effectiveness of these fixed criteria is task-dependent and difficult to generalize across diverse downstream tasks. Perplexity-based data selection provides a simple and model-aware solution to estimate the sample difficulty, but existing approaches typically score the entire training sequence and ignore the difference in learning objectives of language modeling and reasoning tasks. In this paper, we propose PPL-Factory, a simple and interpretable data selection framework that combines task-aware perplexity-based scores and data budget-aware selection criteria. Experiments on GSM8K demonstrate that PPL-Factory outperforms other state-of-the-art data selection methods using only $1\%$ of the training set. With $10\%$ of the data, PPL-Factory exceeds full-data fine-tuning accuracy by 0.9 on GSM8K and 4.8 on MATH. Overall, our results demonstrate that task-aware and budget-aware perplexity-based selection provides an effective and applicable approach for efficient fine-tuning.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.18199v1)
- [PDF](https://arxiv.org/pdf/2607.18199v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/reasoning #keyword/machine-learning #keyword/research-paper
