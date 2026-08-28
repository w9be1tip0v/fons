---
title: "From Static to Dynamic: Benchmarking Real-World Code Review with MCR-Bench"
source: "https://arxiv.org/html/2608.27442v1"
author: "Dewu Zheng, Yanlin Wang, Xiwen Wang, Kefeng Duan, Hongyu Zhang, Xilin Liu, Yuchi Ma, Zibin Zheng"
published: "2026-08-27"
created: 2026-08-29
description: "In real-world software development, code review typically involves iterative interactions between developers and reviewers to improve software quality, making the process costly and time-consuming. Although recent work explores large language models (LLMs) for automated code review, most approaches oversimplify code review into a single-round, static decision task, which fails to capture the multi-round interactive…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
---

# From Static to Dynamic: Benchmarking Real-World Code Review with MCR-Bench

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27442v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27442v1
- pdf:: https://arxiv.org/pdf/2608.27442v1
- categories:: cs.SE, cs.AI, cs.CL

## Abstract / Summary
In real-world software development, code review typically involves iterative interactions between developers and reviewers to improve software quality, making the process costly and time-consuming. Although recent work explores large language models (LLMs) for automated code review, most approaches oversimplify code review into a single-round, static decision task, which fails to capture the multi-round interactive nature and the complex problem-solving processes inherent in realistic review scenarios. To bridge this gap, we introduce MCR-Bench, the first defect state-aware benchmark designed for realistic multi-round code review. MCR-Bench covers five commonly-used programming languages and consists of 2,269 real-world multi-round code review tasks, each of which is annotated with fine-grained defect information and cross-round state labels. Each task in MCR-Bench is equipped with fine-grained defect metadata (e.g., description, type, severity) alongside dynamic state annotations, capturing the complete evolutionary trajectory of a defect throughout the multi-round process. We obtain several findings through extensive experiments on MCR-Bench with mainstream LLMs. (1) Limited overall capability: experiments reveal that mainstream LLMs exhibit limited overall performance in defect detection and defect lifecycle state tracking, with performance degrading significantly as the number of interaction rounds increases; (2) Defect-sensitive performance: LLMs' performance varies substantially across different defect types and severity levels, with semantically complex or low-salience defects being significantly more likely to be missed; (3) Underlying Failure Mechanisms: our in-depth error analysis dissects the distinct drivers of false positives and false negatives, revealing…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27442v1)
- [PDF](https://arxiv.org/pdf/2608.27442v1)
- [RepoReasoner: Evaluating Repository-Level Code Reasoning Ability of Long-Context Language Models](https://arxiv.org/abs/2607.25996) (2026, citations: 2)
- [AACR-Bench: Evaluating Automatic Code Review with Holistic Repository-Level Context](https://arxiv.org/abs/2601.19494) (2026, citations: 5)
- [Sphinx: Benchmarking and Modeling for LLM-Driven Pull Request Review](https://arxiv.org/abs/2601.04252) (2026, citations: 3)
- [Hydra-Reviewer: A Holistic Multi-Agent System for Automatic Code Review Comment Generation](https://www.semanticscholar.org/paper/b38e9ec21d9723ab5fdd8ada646639799ab8ca09) (2025, citations: 8)
- [When More Retrieval Hurts: Retrieval-Augmented Code Review Generation](https://arxiv.org/abs/2511.05302) (2025, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark
