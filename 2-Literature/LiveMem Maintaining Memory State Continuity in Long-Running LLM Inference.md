---
title: "LiveMem: Maintaining Memory State Continuity in Long-Running LLM Inference"
source: "https://arxiv.org/html/2608.02515v1"
author: "Zhichen Liu, Ruihan Sun, Hengjie Yang, Zipeng Wu, Zhaohan Chen, Xiaofan Zhang, Yang Xu"
published: "2026-08-03"
created: 2026-08-05
description: "Long-running assistants and agents consume interaction streams that eventually outgrow the context. Existing context retention, summarization, and retrieval preserve access to selected history, but do not provide a persistent state over the full lifecycle when working context changes. We formulate this missing inference capability as \emph{state continuity under context turnover}: carrying computation forward throug…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/transformer
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/agents
  - keyword/machine-learning
---

# LiveMem: Maintaining Memory State Continuity in Long-Running LLM Inference

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.02515v1)
- published:: 2026-08-03
- updated:: 2026-08-03
- arxiv_id:: 2608.02515v1
- pdf:: https://arxiv.org/pdf/2608.02515v1
- categories:: cs.CL, cs.LG

## Abstract / Summary
Long-running assistants and agents consume interaction streams that eventually outgrow the context. Existing context retention, summarization, and retrieval preserve access to selected history, but do not provide a persistent state over the full lifecycle when working context changes. We formulate this missing inference capability as \emph{state continuity under context turnover}: carrying computation forward through a fixed-capacity memory state whose lifetime is independent of the active context. We introduce an intrinsic memory method, \textbf{LiveMem}, which augments a pretrained full-attention LLM with a memory state that preserves the historical information over the whole lifecycle while the main attention path retains a bounded KV window. Context turnover and memory state maintaining, memory-oriented post-training, and state-aware serving jointly make this memory state load bearing after its originating tokens are released. Our experiments show that LiveMem achieves leading overall performance among evaluated systems and other intrinsic memory methods. Experiments on LongMemEval show that LiveMem is able to answer the question based on the memory state, even when the supporting evidence has been removed from the current context, and evidence-distance analysis shows that useful information persists beyond the active window. LiveMem thus establishes state continuity as a distinct and complementary abstraction for continual LLM inference.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.02515v1)
- [PDF](https://arxiv.org/pdf/2608.02515v1)
- [IndexMem: Learned KV-Cache Eviction with Latent Memory for Long-Context LLM Inference](https://arxiv.org/abs/2605.25475) (2026, citations: 1)
- [Gated DeltaNet-2: Decoupling Erase and Write in Linear Attention](https://arxiv.org/abs/2605.22791) (2026, citations: 12)
- [δ-mem: Efficient Online Memory for Large Language Models](https://arxiv.org/abs/2605.12357) (2026, citations: 3)
- [Understanding LoRA as Knowledge Memory: An Empirical Analysis](https://arxiv.org/abs/2603.01097) (2026, citations: 10)
- [Nested Learning: The Illusion of Deep Learning Architectures](https://arxiv.org/abs/2512.24695) (2025, citations: 75)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/transformer #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/agents #keyword/machine-learning
