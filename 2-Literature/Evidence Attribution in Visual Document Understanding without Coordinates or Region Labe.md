---
title: "Evidence Attribution in Visual Document Understanding without Coordinates or Region Labels"
source: "https://arxiv.org/html/2607.24651v1"
author: "Zhuchenyang Liu, Yao Zhang, Yu Xiao"
published: "2026-07-27"
created: 2026-07-29
description: "Reliable visual document understanding requires a model to attribute each answer to the evidence regions that support it. Recent benchmarks and systems express this step through a coordinate interface: the model outputs the coordinates of bounding boxes that mark the evidence regions in the document. Under this interface, vision-language models often fail to identify the right regions even when the answer is correct…"
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
  - keyword/machine-learning
---

# Evidence Attribution in Visual Document Understanding without Coordinates or Region Labels

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.24651v1)
- published:: 2026-07-27
- updated:: 2026-07-27
- arxiv_id:: 2607.24651v1
- pdf:: https://arxiv.org/pdf/2607.24651v1
- categories:: cs.CV, cs.CL, cs.IR

## Abstract / Summary
Reliable visual document understanding requires a model to attribute each answer to the evidence regions that support it. Recent benchmarks and systems express this step through a coordinate interface: the model outputs the coordinates of bounding boxes that mark the evidence regions in the document. Under this interface, vision-language models often fail to identify the right regions even when the answer is correct, a failure known as Attribution Hallucination. We present a study that investigates whether this failure is partially limited by what the model can express through coordinates. On a verified bilingual CiteVQA subset, we compare the coordinate interface with a language interface in which the model outputs only text, quoting its evidence verbatim, and a multimodal retriever returns the location of each quote as a page region proposed by a layout parser (tables and figures are quoted through their captions or notes); the comparison is repeated over six open vision-language models. Compared with the coordinate interface, evidence recall rises from at most 8 points to between 26 and 47 and the hallucination rate roughly halves, with little change in answer quality. Building on this comparison, we use the same quote-and-retrieve pipeline as a training scaffold: because region-level evidence labels are expensive to collect for long documents, we introduce a GRPO recipe whose reward is a judge's reading of the gold answer and crops of the retrieved regions, training the model to quote better evidence without any region labels and raising an 8B backbone's strict attributed accuracy from 22.4 to 33.8. These findings indicate a practical path to improve attribution"without a coordinate interface and without costly region-level supervision.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.24651v1)
- [PDF](https://arxiv.org/pdf/2607.24651v1)
- [CiteVQA: Benchmarking Evidence Attribution for Trustworthy Document Intelligence](https://arxiv.org/abs/2605.12882) (2026, citations: 2)
- [HART: High-Resolution Annotation-Free Reasoning Technique through a Closed-loop Framework](https://arxiv.org/abs/2602.23615) (2026, citations: 3)
- [Qwen3-VL-Embedding and Qwen3-VL-Reranker: A Unified Framework for State-of-the-Art Multimodal Retrieval and Ranking](https://arxiv.org/abs/2601.04720) (2026, citations: 149)
- [DocR1: Evidence Page-Guided GRPO for Multi-Page Document Understanding](https://arxiv.org/abs/2508.07313) (2025, citations: 11)
- [Correctness is not Faithfulness in Retrieval Augmented Generation Attributions](https://www.semanticscholar.org/paper/cdfe1fd4bae2e2e2b335621e3f97d5b963be3870) (2025, citations: 27)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/evaluation #keyword/benchmark #keyword/machine-learning
