---
title: "Native-speed vLLM transformers modeling backend"
source: "https://huggingface.co/blog/native-speed-vllm-transformers-backend"
author: "Hugging Face Blog"
published: "2026-07-08"
created: 2026-07-13
description: "Hugging Face reports that the transformers modeling backend for vLLM now matches or beats custom native vLLM implementations for many LLM architectures by applying torch.fx/AST layer fusions at runtime, so model authors get fast inference without a separate custom port."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/transformer
  - keyword/language-model
  - keyword/inference
  - keyword/machine-learning
  - keyword/evaluation
---

# Native-speed vLLM transformers modeling backend

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/native-speed-vllm-transformers-backend)
- published:: 2026-07-08

## Abstract / Summary
The transformers backend in vLLM previously focused on plugging efficient attention while leaving other inference optimizations to hand-written vLLM ports. This update uses torch.fx static analysis and AST rewriting to fuse operations into optimized vLLM kernels (including MoE expert-parallel paths and parallel linear layers), remaining compatible with torch.compile and CUDA Graphs. Benchmarks on Qwen3-4B, Qwen3-32B, and Qwen3-235B-A22B-FP8 show the transformers backend meeting or beating native throughput. Serving uses `--model-impl transformers` alongside existing tensor/data/expert parallelism flags, reducing the need for a separate custom model port after a transformers implementation lands.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/transformer #keyword/language-model #keyword/inference #keyword/machine-learning #keyword/evaluation
