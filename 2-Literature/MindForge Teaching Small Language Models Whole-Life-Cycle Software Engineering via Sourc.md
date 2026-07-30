---
title: "MindForge: Teaching Small Language Models Whole-Life-Cycle Software Engineering via Source-Free Program Synthesis"
source: "https://arxiv.org/html/2607.27146v1"
author: "Yihao Chen, Shi Chang, Khaled Chawa, Feng Lin, Boyuan Chen, Shaowei Wang, Ahmed E. Hassan"
published: "2026-07-29"
created: 2026-07-31
description: "Coding agents have made substantial progress on software engineering tasks that modify existing codebases, including bug fixing and feature implementation. However, constructing a complete program from scratch remains a major challenge: even the frontier models evaluated on ProgramBench fully resolve fewer than 1% of tasks. One obstacle is the lack of scalable training environments for this from-scratch setting, spa…"
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

# MindForge: Teaching Small Language Models Whole-Life-Cycle Software Engineering via Source-Free Program Synthesis

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.27146v1)
- published:: 2026-07-29
- updated:: 2026-07-29
- arxiv_id:: 2607.27146v1
- pdf:: https://arxiv.org/pdf/2607.27146v1
- categories:: cs.SE, cs.CL, cs.LG

## Abstract / Summary
Coding agents have made substantial progress on software engineering tasks that modify existing codebases, including bug fixing and feature implementation. However, constructing a complete program from scratch remains a major challenge: even the frontier models evaluated on ProgramBench fully resolve fewer than 1% of tasks. One obstacle is the lack of scalable training environments for this from-scratch setting, spanning the whole software engineering life cycle, as existing environment-construction frameworks focus only on a single phase in software development. To address this gap, we introduce MindForge, an automated pipeline that converts open-source command-line programs into source-free environments that expose only a compiled reference executable and its documentation. Using MindForge, we construct training environments from repositories disjoint from those in ProgramBench, and curate a high-quality data recipe consisting of program synthesis trajectories using GLM-5.2 as the teacher agent. Fine-tuning Qwen3.6-27B on these trajectories increases its ProgramBench average test pass rate from 37.98% to 49.51%, achieving performance comparable to substantially larger frontier models. Moreover, the fine-tuned model consistently improves over the base model across all seven unseen software engineering benchmarks, spanning long-horizon repository generation and translation, bug fixing, feature implementation, and cross-language issue resolution, with absolute gains of 31.00 points on RepoZero-C2Rust, 14.16 on DeepSWE, 10.70/4.56 on NL2Repo-Bench (with/without tests), 5.04 on SWE-bench Verified, 5.93 on SWE-bench Pro, 5.22 on SWE-bench Multilingual, and 4.94 on FeatBench.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.27146v1)
- [PDF](https://arxiv.org/pdf/2607.27146v1)
- [DeepSWE: Measuring Frontier Coding Agents on Original, Long-Horizon Engineering Tasks](https://arxiv.org/abs/2607.07946) (2026, citations: 9)
- [OpenThoughts-Agent: Data Recipes for Agentic Models](https://arxiv.org/abs/2606.24855) (2026, citations: 2)
- [DeNovoSWE: Scaling Long-Horizon Environments for Generating Entire Repositories from Scratch](https://arxiv.org/abs/2606.10728) (2026, citations: 1)
- [RepoZero: Can LLMs Generate a Code Repository from Scratch?](https://arxiv.org/abs/2605.07122) (2026, citations: 4)
- [ProgramBench: Can Language Models Rebuild Programs From Scratch?](https://arxiv.org/abs/2605.03546) (2026, citations: 19)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/machine-learning
