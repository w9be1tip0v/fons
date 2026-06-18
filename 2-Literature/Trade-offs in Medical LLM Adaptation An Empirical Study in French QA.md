---
title: "Trade-offs in Medical LLM Adaptation: An Empirical Study in French QA"
source: "https://arxiv.org/html/2606.19266v1"
author: "Ikram Belmadani, Oumaima El Khettari, Carlos Ramisch, Frederic Bechet, Richard Dufour, Benoit Favre"
published: "2026-06-17"
created: 2026-06-19
description: "The development of large language models (LLMs) has led to an increased focus on their adaptation to specialized domains and languages, yet the effectiveness of domain adaptation strategies remains unclear. We present a study of medical domain adaptation using French medical question-answering (QA) as a case study. We compare continual pretraining (CPT), supervised fine-tuning (SFT), and their combination across thr…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
---

# Trade-offs in Medical LLM Adaptation: An Empirical Study in French QA

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.19266v1)
- published:: 2026-06-17
- updated:: 2026-06-17
- arxiv_id:: 2606.19266v1
- pdf:: https://arxiv.org/pdf/2606.19266v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
The development of large language models (LLMs) has led to an increased focus on their adaptation to specialized domains and languages, yet the effectiveness of domain adaptation strategies remains unclear. We present a study of medical domain adaptation using French medical question-answering (QA) as a case study. We compare continual pretraining (CPT), supervised fine-tuning (SFT), and their combination across three model families, multiple sizes, and three initialization types, explicitly disentangling adaptation effects from base model choice. We evaluate both multiple-choice (MCQA) and open-ended QA (OEQA) under greedy and constrained decoding using automatic metrics and LLM-as-a-Judge evaluation. For MCQA, CPT+SFT most often achieves the best scores, but gains over SFT are small and frequently not statistically significant, making SFT a strong and cost-effective default. For OEQA, CPT consistently improves overlap-based metrics, while SFT often degrades generation quality; instruction tuning and CPT+SFT are preferred by LLM-based evaluation. Cross-lingual experiments further show effective transfer from French adaptation to English benchmarks. Overall, we provide practical guidelines for selecting adaptation strategies under computational constraints.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.19266v1)
- [PDF](https://arxiv.org/pdf/2606.19266v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/machine-learning
