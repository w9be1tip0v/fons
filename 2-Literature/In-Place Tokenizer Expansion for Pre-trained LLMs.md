---
title: "In-Place Tokenizer Expansion for Pre-trained LLMs"
source: "https://arxiv.org/html/2607.15232v1"
author: "Jimmy T. H. Smith, Tarek Dakhran, Alberto Cabrera, Simon S. Lee, Paul Pak, Aditya Tadimeti, Tim Seyde, Maxime Labonne, Alexander Amini, Mathias Lechner"
published: "2026-07-16"
created: 2026-07-17
description: "In-place BPE tokenizer expansion for pretrained models: continue merges, mean-init new embeddings, two-stage adaptation; cuts Hindi/Vietnamese tokens ~2.4–2.6× on LFM2-family MoE."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/llm
  - keyword/fine-tuning
  - keyword/inference
---

# In-Place Tokenizer Expansion for Pre-trained LLMs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15232v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15232v1
- pdf:: https://arxiv.org/pdf/2607.15232v1
- categories:: cs.CL

## Abstract / Summary
Tokenizers fixed at pretraining fragment languages added later, raising latency and energy for those users. Tokenizer expansion continues the existing BPE merges on a multilingual corpus so most source tokens carry over unchanged and every new token has an exact source decomposition. Carried-over embeddings are copied; new rows are mean-initialized from source sub-tokens. Embedding-only then full continued pretraining recovers quality. Applied to LFM2-8B-A1B toward LFM2.5-8B-A1B (128K vocab): Hindi/Vietnamese use ~2.4×/2.6× fewer tokens (up to 4.0× Thai), estimating 2.2–3.7× per-character decode speedup. Weights and tokenizer released.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15232v1)
- [PDF](https://arxiv.org/pdf/2607.15232v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/llm #keyword/fine-tuning #keyword/inference
