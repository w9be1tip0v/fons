---
title: "TokTier: Exact Stateful Tokenization for Agentic LLM Serving"
source: "https://arxiv.org/html/2607.29678v1"
author: "Zhenyu Zhang, Zhichao Cao"
published: "2026-07-31"
created: 2026-08-04
description: "LLM serving systems cache prompt KV state, yet most front ends still re-tokenize the full request text on every call. The cost lands on coding agents, which resubmit a long transcript after each small tool result, and reuse is hard because even a short append can change token boundaries near the end of the previous sequence. Across 153,951 calls from two agent ecosystems, the median call appends about 1.4K character…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/agents
---

# TokTier: Exact Stateful Tokenization for Agentic LLM Serving

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.29678v1)
- published:: 2026-07-31
- updated:: 2026-07-31
- arxiv_id:: 2607.29678v1
- pdf:: https://arxiv.org/pdf/2607.29678v1
- categories:: cs.CL, cs.DC, cs.PF

## Abstract / Summary
LLM serving systems cache prompt KV state, yet most front ends still re-tokenize the full request text on every call. The cost lands on coding agents, which resubmit a long transcript after each small tool result, and reuse is hard because even a short append can change token boundaries near the end of the previous sequence. Across 153,951 calls from two agent ecosystems, the median call appends about 1.4K characters, and only 1.0-3.6% of calls start or rebuild a session with contexts of millions of characters. At a 94.1% fleet prompt-cache hit rate, tokenization reaches up to 64% of time to first token. TokTier is a stateful tokenization service with one contract: emitted token IDs are always identical to full reference tokenization of the request text. For a session continuation, it re-tokenizes a small window around the append and splices only after a per-request stable-boundary check, widening the window or falling back to full tokenization on failure. For a call without a reusable prefix, it decomposes GPT-family regex pre-tokenization into run-local rules and runs exact pre-tokenization and BPE on a GPU. A sampled shadow verifier re-checks live traffic. Across 17 tokenizer families, differential campaigns cover 1.5x10^10 split checks, a 12.4 TB real-text corpus, and 93,000+ replayed agent steps, with zero divergence. Incremental repair takes 0.5-1.1 ms from 100K to 3M characters, up to 437x faster than HF tokenization and 2.1x faster at 1M than the strongest cache-based baseline (Gigatoken) fully prewarmed. GPU full tokenization encodes a 1M-character request in 0.87 ms, up to 491x below HF and 23.4x below the fastest published CPU method. With vLLM, median time to first token drops 16-34% and P99 drops 23% under recorded bursts. Under a 50 ms P99 objective, four…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.29678v1)
- [PDF](https://arxiv.org/pdf/2607.29678v1)
- [CacheWise: Understanding Workloads and Optimizing KVCache Management for Efficiently Serving LLM Coding Agents](https://arxiv.org/abs/2606.16824) (2026, citations: 3)
- [GPUTOK: GPU Accelerated Byte Level BPE Tokenization](https://arxiv.org/abs/2603.02597) (2026, citations: 1)
- [BurstGPT: A Real-World Workload Dataset to Optimize LLM Serving Systems](https://arxiv.org/abs/2401.17644) (2024, citations: 120)
- [DistServe: Disaggregating Prefill and Decoding for Goodput-optimized Large Language Model Serving](https://arxiv.org/abs/2401.09670) (2024, citations: 817)
- [SGLang: Efficient Execution of Structured Language Model Programs](https://arxiv.org/abs/2312.07104) (2023, citations: 1143)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/agents
