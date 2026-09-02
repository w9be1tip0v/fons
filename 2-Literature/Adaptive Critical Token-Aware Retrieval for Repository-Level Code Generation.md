---
title: "Adaptive Critical Token-Aware Retrieval for Repository-Level Code Generation"
source: "https://arxiv.org/html/2609.01601v1"
author: "Kefeng Duan, Dewu Zheng, Yanlin Wang, Terry Yue Zhuo, Mingwei Liu, Jianxing Yu, Jiachi Chen, Ensheng Shi, Xilin Liu, Yuchi Ma, Zibin Zheng"
published: "2026-09-01"
created: 2026-09-03
description: "The repository-level code generation task requires synthesizing code that satisfies task requirements while remaining consistent with the target repository context. Since real-world repositories often exceed the input length limits of LLMs, existing approaches commonly adopt retrieval-augmented generation (RAG) to provide repository-specific context. Despite improving repository-context retrieval, existing methods t…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/research-paper
---

# Adaptive Critical Token-Aware Retrieval for Repository-Level Code Generation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.01601v1)
- published:: 2026-09-01
- updated:: 2026-09-01
- arxiv_id:: 2609.01601v1
- pdf:: https://arxiv.org/pdf/2609.01601v1
- categories:: cs.SE, cs.AI, cs.CL

## Abstract / Summary
The repository-level code generation task requires synthesizing code that satisfies task requirements while remaining consistent with the target repository context. Since real-world repositories often exceed the input length limits of LLMs, existing approaches commonly adopt retrieval-augmented generation (RAG) to provide repository-specific context. Despite improving repository-context retrieval, existing methods typically provide context as task-level support, without explicitly identifying the critical tokens that require fine-grained repository context during generation. During the autoregressive generation process of LLMs, errors often concentrate at a small number of decisive positions: once such tokens are generated incorrectly, subsequent code may follow an incorrect semantic path and eventually lead to functional failure. We refer to these positions as "critical tokens". In this paper, we propose ACToR, an adaptive critical token-aware retrieval framework for repository-level code generation. ACToR identifies critical tokens during generation and triggers targeted retrieval on demand to provide repository context at these decisive positions. In addition, we design a position-aware weighting method for dense retrievers to prioritize context that is more informative for generation. We evaluate ACToR on two representative repository-level benchmarks, RepoExec and CoderEval. Experimental results show that ACToR consistently outperforms state-of-the-art methods, achieving relative improvements of 8.4% on RepoExec and 15.4% on CoderEval. Beyond performance gains, we systematically quantify the impact of critical tokens, revealing their central role in major generation failures and highlighting the necessity of targeted retrieval strategies. We provide the code and d…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.01601v1)
- [PDF](https://arxiv.org/pdf/2609.01601v1)
- [SWE-Prime: Fewer Trajectories, Better Performance](https://arxiv.org/abs/2608.27449) (2026, citations: 1)
- [PhoenixRepair: Rethinking Repair Strategy Exploration in Software Agents](https://arxiv.org/abs/2607.18859) (2026, citations: 2)
- [RepoReasoner: Evaluating Repository-Level Code Reasoning Ability of Long-Context Language Models](https://arxiv.org/abs/2607.25996) (2026, citations: 4)
- [RealSec-bench: A Benchmark for Evaluating Secure Code Generation in Real-World Repositories](https://arxiv.org/abs/2601.22706) (2026, citations: 12)
- [ShortCoder: Knowledge-Augmented Syntax Optimization for Token-Efficient Code Generation](https://arxiv.org/abs/2601.09703) (2026, citations: 4)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/research-paper
