---
title: "HalluTruthQA-4K: A Fine-Grained Corpus and Annotation Process for Arabic Hallucination Detection and Truth Verification"
source: "https://arxiv.org/html/2608.03966v1"
author: "Salah Eddine Bekhouche, Abdessalam Bouchekif, Hichem Telli, Mohammed-En-Nadhir Zighem, Abdenour Hadid"
published: "2026-08-04"
created: 2026-08-06
description: "Large language models can generate fluent Arabic answers while introducing factual errors that are difficult to identify and verify. Existing Arabic hallucination resources often assign a binary label to an entire response, indicating whether it is hallucinated or non-hallucinated, but provide limited information about the exact erroneous content, the reason for the error, or the correct factual answer. We present H…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
---

# HalluTruthQA-4K: A Fine-Grained Corpus and Annotation Process for Arabic Hallucination Detection and Truth Verification

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.03966v1)
- published:: 2026-08-04
- updated:: 2026-08-04
- arxiv_id:: 2608.03966v1
- pdf:: https://arxiv.org/pdf/2608.03966v1
- categories:: cs.CL

## Abstract / Summary
Large language models can generate fluent Arabic answers while introducing factual errors that are difficult to identify and verify. Existing Arabic hallucination resources often assign a binary label to an entire response, indicating whether it is hallucinated or non-hallucinated, but provide limited information about the exact erroneous content, the reason for the error, or the correct factual answer. We present HalluTruthQA-4K, an expanded version of the HalluTruthQA resource containing 4,000 expert-curated Arabic question-answering instances across four knowledge-intensive domains: Islamic knowledge, history, science, and geography. Serving as the official dataset for Track 2 of the HalluScoring 2026 shared task, HalluTruthQA-4K extends our original corpus to 4,000 instances. Each instance pairs an Arabic question with a model-generated response, a verified reference answer, and five plausible distractors. Hallucinated responses are additionally annotated with character-level erroneous spans, human-written explanations, and hierarchical hallucination types. The corpus contains 1,643 hallucinated and 2,357 non-hallucinated responses, with 1,843 annotated erroneous spans. We describe the resource construction and annotation methodology, including question selection, controlled answer generation, candidate construction, expert annotation, independent verification, adjudication, and quality control. We also document the annotation guidelines, taxonomy, data format, inter-annotator agreement, and corpus statistics. HalluTruthQA-4K provides a reusable resource for hallucination detection, span-level error localization, explanation generation, factual verification, and the broader evaluation of factual reliability in Arabic language models.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.03966v1)
- [PDF](https://arxiv.org/pdf/2608.03966v1)
- [HalluTruthQA: A Fine-Grained Benchmark for Hallucination Detection, Localization, and Explanation in Arabic Question Answering](https://arxiv.org/abs/2607.20219) (2026, citations: 2)
- [HalluScore: Large Language Model Hallucination Question Answering Benchmark](https://arxiv.org/abs/2605.17007) (2026, citations: 2)
- [QIAS 2026: Overview of the Shared Task on Islamic Inheritance Reasoning](https://arxiv.org/abs/2606.13756) (2026, citations: 4)
- [IslamicMMLU: A Benchmark for Evaluating LLMs on Islamic Knowledge](https://arxiv.org/abs/2603.23750) (2026, citations: 3)
- [MAWARITH: A Dataset and Benchmark for Legal Inheritance Reasoning with LLMs](https://arxiv.org/abs/2603.07539) (2026, citations: 7)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation
