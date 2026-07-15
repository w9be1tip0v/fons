---
title: "Knowledgeless Language Models: Suppressing Parametric Recall for Evidence-Grounded Language Modeling"
source: "https://arxiv.org/html/2607.12831v1"
author: "Roi Cohen, Yvan Carré, Nick Lechtenbörger, Hendrik Droste, Lucas Kerschke, Russa Biswas, Gerard de Melo, Jan Buys"
published: "2026-07-14"
created: 2026-07-16
description: "KLLMs are pretrained with entity-anonymized corpora to suppress parametric factual recall and improve evidence-grounded QA, fact verification, hallucination detection, calibration, and robustness under imperfect retrieval."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/ai
  - keyword/retrieval
  - keyword/evaluation
  - keyword/safety
  - keyword/machine-learning
  - keyword/research-paper
---

# Knowledgeless Language Models: Suppressing Parametric Recall for Evidence-Grounded Language Modeling

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.12831v1)
- published:: 2026-07-14
- updated:: 2026-07-14
- arxiv_id:: 2607.12831v1
- pdf:: https://arxiv.org/pdf/2607.12831v1
- categories:: cs.CL, cs.LG

## Abstract / Summary
Language models encode substantial factual knowledge in their parameters, which can lead to unreliable behavior when this knowledge is outdated, incomplete, or misaligned with the provided context. In this work, we study whether modifying the pretraining signal can systematically shift models away from parametric recall and toward evidence-grounded reasoning. We introduce Knowledge-Less Language Models (KLLMs), a fundamentally different epistemic training paradigm for LLMs, which are pretrained on corpora in which named entities are anonymized, thereby removing a primary channel for entity-linked factual supervision. This intervention substantially reduces closed-book factual recall, while often improving performance on tasks where relevant information is provided as context. Across multiple model scales, KLLMs consistently outperform matched baselines on contextual question answering, fact verification, and hallucination detection benchmarks. Crucially, in retrieval-grounded settings with imperfect evidence, KLLMs show improved robustness and achieve up to 20--25% relative gains over standard language models. They further exhibit better calibration, with improved ECE, Brier score, and AUROC, as well as more reliable abstention behavior. Our results demonstrate that suppressing entity-linked supervision during pretraining induces a shift in epistemic behavior: KLLMs rely less on parametric knowledge and more on external evidence, leading to improved reliability under realistic conditions. This suggests that pretraining-time control over knowledge acquisition can complement retrieval-augmented and tool-based systems by providing a more evidence-sensitive base model.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.12831)
- [PDF](https://arxiv.org/pdf/2607.12831v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/ai #keyword/retrieval #keyword/evaluation #keyword/safety #keyword/machine-learning #keyword/research-paper
