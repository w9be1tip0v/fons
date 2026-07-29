---
title: "Evaluating Multi-Turn Multimodal Diagnostic Reasoning on Challenging Real-World Clinical Cases"
source: "https://arxiv.org/html/2607.25933v1"
author: "Rui Yang, Weihao Xuan, Yi Lin, Zhuhan Bao, Jonathan Chong Kai Liew, Matthew Yu Heng Wong, Nicolás Lescano, Nikita R. Paripati, Emily Ling-Lin Pai, Jiarui Liu, Heli Qi, Heng-Jui Chang, Benny Kai Guo Loo, Huitao Li, Kunyu Yu, Yufan Wang, Chuan Hong, Shijian Lu, Douglas Teodoro, Naoto Yokoya, Ross Koppel, Mona Diab, Hua Xu, David W. Bates, Nan Liu, Yifan Peng"
published: "2026-07-28"
created: 2026-07-30
description: "Clinical diagnostic evaluation should not only assess whether models can provide correct diagnoses, but also reflect the realities of clinical practice, including progressive disclosure of multimodal information, dynamic updating of diagnostic hypotheses, and continuous refinement of clinical reasoning. However, existing evaluations of multimodal large language models (MLLMs) typically rely on single-turn or isolate…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
---

# Evaluating Multi-Turn Multimodal Diagnostic Reasoning on Challenging Real-World Clinical Cases

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.25933v1)
- published:: 2026-07-28
- updated:: 2026-07-28
- arxiv_id:: 2607.25933v1
- pdf:: https://arxiv.org/pdf/2607.25933v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Clinical diagnostic evaluation should not only assess whether models can provide correct diagnoses, but also reflect the realities of clinical practice, including progressive disclosure of multimodal information, dynamic updating of diagnostic hypotheses, and continuous refinement of clinical reasoning. However, existing evaluations of multimodal large language models (MLLMs) typically rely on single-turn or isolated tasks, making it difficult to fully capture the complexity of real-world clinical diagnosis. To bridge this gap, we developed ClinMM-Bench, the largest multi-turn multimodal clinical diagnostic evaluation benchmark to date. ClinMM-Bench contains 1,089 challenging real-world clinical cases and 3,760 medical images across eight specialties. We systematically evaluated 15 representative MLLMs using a two-level evaluation framework that assessed both diagnostic accuracy and diagnostic reasoning quality. Results showed that proprietary models achieved the highest overall diagnostic accuracy, but the proportion of completely correct diagnoses remained limited across all models. In terms of diagnostic reasoning quality, current models can identify plausible diagnostic directions but still have considerable limitations in generating reliable diagnostic reasoning. Error analysis further identified five representative failure modes: information synthesis failure, knowledge mapping error, perception error, premature closure, and visual hallucination.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.25933v1)
- [PDF](https://arxiv.org/pdf/2607.25933v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/evaluation #keyword/benchmark #keyword/reasoning
