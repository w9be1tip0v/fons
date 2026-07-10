---
title: "Profiling in PyTorch (Part 3): Attention is all you profile"
source: "https://huggingface.co/blog/torch-attention-profile"
author: "Hugging Face Blog"
published: "2026-07-10"
created: 2026-07-11
description: "This is the third post of Profiling in PyTorch, a series where we slowly build the skill of reading profiler traces and use it to drive optimization: The series 'Profiling in PyTorch' is meant to make you comfortable reading profiler traces and tables. In Part 1 we profiled basic math operations like addition and multiplication. We saw how the profiler table uncovers hotspots, and how the profiler trace shows the or…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/transformer
---

# Profiling in PyTorch (Part 3): Attention is all you profile

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/torch-attention-profile)
- published:: 2026-07-10

## Abstract / Summary
This is the third post of Profiling in PyTorch, a series where we slowly build the skill of reading profiler traces and use it to drive optimization: The series "Profiling in PyTorch" is meant to make you comfortable reading profiler traces and tables. In Part 1 we profiled basic math operations like addition and multiplication. We saw how the profiler table uncovers hotspots, and how the profiler trace shows the order in which an algorithm runs over time. In Part 2 we wrapped that addition and multiplication into a torch linear layer. We then stacked several linear layers on top of each other (a multilayer perceptron) and profiled that. Along the way we also profiled fused and hand-tuned kernels. From the perspective of the Transformer architecture, the next logical step for us to profile is yet another fundamental algorithm, attention. While being infamous for its quadratic-time complexity, many clever tricks exist to mitigate that issue and make it fast. Our goal here is not to cover every trick in detail. Instead, we want to see how each one looks different under the profiler. The scripts for this blog post live here: 04_a_naive_attention.py , 04_b_inplace_ops_attention.py , 0…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/transformer
