---
title: "OmegaUse-OfficeVal: Benchmarking LLM Agents on Long-Horizon Office-Suite Tasks with Economic Grounding"
source: "https://arxiv.org/html/2607.27155v1"
author: "Jingbo Zhou, Yusai Zhao, Qi Bao, Jingjia Cao, Zhenghai Chen, Chang Gao, Kaiqi Guo, Muxin Guo, Mingxuan Li, Xinjiang Lu, Yanru Ma, Yixiong Xiao, Zenghui Zhang, Le Zhang, Hua Wu"
published: "2026-07-29"
created: 2026-07-31
description: "Large language model (LLM) agents are increasingly expected to assist users in completing tasks. However, existing benchmarks provide limited support for evaluating whether agents can carry out office-suite workflows at a reasonable cost. We introduce OmegaUse-OfficeVal, a benchmark for evaluating LLM agents on long-horizon office-suite tasks with task-level economic grounding. The benchmark comprises 100 tasks deri…"
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
  - keyword/agents
  - keyword/machine-learning
---

# OmegaUse-OfficeVal: Benchmarking LLM Agents on Long-Horizon Office-Suite Tasks with Economic Grounding

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.27155v1)
- published:: 2026-07-29
- updated:: 2026-07-29
- arxiv_id:: 2607.27155v1
- pdf:: https://arxiv.org/pdf/2607.27155v1
- categories:: cs.AI, cs.CL, cs.HC

## Abstract / Summary
Large language model (LLM) agents are increasingly expected to assist users in completing tasks. However, existing benchmarks provide limited support for evaluating whether agents can carry out office-suite workflows at a reasonable cost. We introduce OmegaUse-OfficeVal, a benchmark for evaluating LLM agents on long-horizon office-suite tasks with task-level economic grounding. The benchmark comprises 100 tasks derived from office-suite requests proposed by practitioners and adapted through a privacy-preserving process. On average, these tasks require 2.32 hours of human labor to complete. An important feature of the benchmark is that each task is paired with two economic signals: human labor time and task price proxy. These signals enable direct comparisons between human costs and LLM inference costs, as well as value-weighted evaluation. To support stable evaluation, we develop code-based verifiers from fine-grained rubrics. We evaluate several frontier LLMs together with a human baseline. Although all evaluated LLMs are substantially cheaper and faster than human workers, they have not yet approached human-level deliverable quality. The code and dataset are fully open-sourced, and more information is available on our project website: https://omegause-officeval.github.io.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.27155v1)
- [PDF](https://arxiv.org/pdf/2607.27155v1)
- [DocOps: A Verifiable Benchmark for Autonomous Agents in Complex Document Operations](https://arxiv.org/abs/2607.19865) (2026, citations: 1)
- [PPT-Eval: A Benchmark for Computer-Use Agents on PowerPoint Tasks](https://arxiv.org/abs/2606.31154) (2026, citations: 3)
- [MiniMax Sparse Attention](https://arxiv.org/abs/2606.13392) (2026, citations: 6)
- [WindowsWorld: A Process-Centric Benchmark of Autonomous GUI Agents in Professional Cross-Application Environments](https://arxiv.org/abs/2604.27776) (2026, citations: 6)
- [DeepSeek-V4: Towards Highly Efficient Million-Token Context Intelligence](https://arxiv.org/abs/2606.19348) (2026, citations: 422)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/machine-learning
