---
title: "Gradient-free Task-Conditioned Retrieval for On-Device In-Context Learning"
source: "https://arxiv.org/html/2607.27766v1"
author: "Xinyu Luo, Hui Liu, Yihua Shao, Junyi Yang, Arindam Basu, Haoliang Li"
published: "2026-07-30"
created: 2026-08-03
description: "On-device in-context learning (ICL) relies on pre-inference retrieval to select demonstrations for useful context before downstream model inference. This retrieval must exploit task-specific information while operating over local memories under limited computation, memory, and data-exposure budgets. We propose Conditional Retrieval Alignment (CoRA), a gradient-free framework that converts a frozen encoder into a tas…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/safety
  - keyword/machine-learning
---

# Gradient-free Task-Conditioned Retrieval for On-Device In-Context Learning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.27766v1)
- published:: 2026-07-30
- updated:: 2026-07-30
- arxiv_id:: 2607.27766v1
- pdf:: https://arxiv.org/pdf/2607.27766v1
- categories:: cs.CL, cs.IR, cs.LG

## Abstract / Summary
On-device in-context learning (ICL) relies on pre-inference retrieval to select demonstrations for useful context before downstream model inference. This retrieval must exploit task-specific information while operating over local memories under limited computation, memory, and data-exposure budgets. We propose Conditional Retrieval Alignment (CoRA), a gradient-free framework that converts a frozen encoder into a task-conditioned retriever using paired candidate inputs and outputs. CoRA selects complementary encoder layers, constructs an output-derived conditioning space from candidate memory, and aligns candidate input representations to this space through closed-form ridge regression. Low-rank factorization then produces a compact retrieval basis where candidate outputs are used only during offline index construction, whereas query-time retrieval requires only the query input and precomputed index. We show that CoRA's rank-constrained basis is the optimal low-rank compression of the output-conditioned fitted representation, and derive an exact two-pass streaming construction that avoids materializing the full fitted matrix. We further extend the framework to multimodal exemplar retrieval by incorporating visual representations into the conditioning and retrieval spaces. Experiments across ten textual datasets and four multimodal benchmarks with Llama-3.2-1B, MobileLLM-Pro, OpenFlamingo-3B, and Qwen3.5-2B, as well as end-to-end Raspberry Pi~5 deployment demonstrate that CoRA supports effective task-conditioned retrieval without retriever fine-tuning, backpropagation, or target-model calls.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.27766v1)
- [PDF](https://arxiv.org/pdf/2607.27766v1)
- [MobileLLM-Pro Technical Report](https://arxiv.org/abs/2511.06719) (2025, citations: 3)
- [Precise and scalable analogue matrix equation solving using resistive random-access memory chips](https://www.nature.com/articles/s41928-025-01477-0.pdf) (2025, citations: 22)
- [PICK: An SRAM-based Processing-in-Memory Accelerator for K-Nearest-Neighbor Search in Point Clouds](https://www.semanticscholar.org/paper/41f608548ab0ba6eaa5c2e15158e8e475e95d7d6) (2025, citations: 2)
- [Provoking Multi-modal Few-Shot LVLM via Exploration-Exploitation In-Context Learning](https://arxiv.org/abs/2506.09473) (2025, citations: 4)
- [Qwen3 Embedding: Advancing Text Embedding and Reranking Through Foundation Models](https://arxiv.org/abs/2506.05176) (2025, citations: 1147)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/safety #keyword/machine-learning
