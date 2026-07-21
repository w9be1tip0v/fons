---
title: "SWE-Pruner Pro: The Coder LLM Already Knows What to Prune"
source: "https://arxiv.org/html/2607.18213v1"
author: "Yuhang Wang, Yuling Shi, Shaoqiu Zhang, Jialiang Liang, Shilin He, Siyu Ye, Yuting Chen, Kai Cai, Xiaodong Gu"
published: "2026-07-20"
created: 2026-07-22
description: "Pruning long context for coding agents has been a vital technology for efficient context management. While existing context pruning methods such as SWE-Pruner realize this by attaching a separate code classifier, we find the agent itself encodes internal representations indicating the relevance of code context when reading tool output. Based on this finding, we propose SWE-Pruner Pro, which prunes tool outputs direc…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
  - keyword/machine-learning
---

# SWE-Pruner Pro: The Coder LLM Already Knows What to Prune

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.18213v1)
- published:: 2026-07-20
- updated:: 2026-07-20
- arxiv_id:: 2607.18213v1
- pdf:: https://arxiv.org/pdf/2607.18213v1
- categories:: cs.CL, cs.SE

## Abstract / Summary
Pruning long context for coding agents has been a vital technology for efficient context management. While existing context pruning methods such as SWE-Pruner realize this by attaching a separate code classifier, we find the agent itself encodes internal representations indicating the relevance of code context when reading tool output. Based on this finding, we propose SWE-Pruner Pro, which prunes tool outputs directly inside the agent. Concretely, a small head turns the agent's own internal representations into a keep-or-prune label for each line, with a length-aware embedding keyed to each tool output's line count. Across two open-weight backbones and four multi-turn benchmarks, SWE-Pruner Pro saves up to 39% of prompt and completion tokens while preserving task quality, with bounded inference overhead. Notably, on MiMo-V2-Flash SWE-Pruner Pro additionally raises the SWE-Bench Verified resolve rate by +3.8% and the long-context Oolong accuracy by +2.2 points.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.18213v1)
- [PDF](https://arxiv.org/pdf/2607.18213v1)
- [SWE-MeM: Learning Adaptive Memory Management for Long-Horizon Coding Agents](https://arxiv.org/abs/2606.28434) (2026, citations: 1)
- [FastContext: Training Efficient Repository Explorer for Coding Agents](https://arxiv.org/abs/2606.14066) (2026, citations: 1)
- [SWE-Explore: Benchmarking How Coding Agents Explore Repositories](https://arxiv.org/abs/2606.07297) (2026, citations: 4)
- [ClassEval-Pro: A Cross-Domain Benchmark for Class-Level Code Generation](https://arxiv.org/abs/2604.26923) (2026, citations: 2)
- [SWE-QA-Pro: A Representative Benchmark and Scalable Training Recipe for Repository-Level Code Understanding](https://arxiv.org/abs/2603.16124) (2026, citations: 3)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/machine-learning
