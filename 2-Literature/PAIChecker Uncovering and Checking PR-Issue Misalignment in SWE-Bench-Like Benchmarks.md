---
title: "PAIChecker: Uncovering and Checking PR-Issue Misalignment in SWE-Bench-Like Benchmarks"
source: "https://arxiv.org/html/2607.28587v1"
author: "Manyi Wang, Junjielong Xu, Pinjia He"
published: "2026-07-30"
created: 2026-08-02
description: "SWE-bench-like benchmarks are widely used for evaluating LLM's issue resolution capability. They typically follow a common construction pipeline: each PR (Pull Request) is paired with its linked issue by extracting issue references from the PR description; the issue description is used as the problem statement, and the PR patch serves as the test oracle. However, due to the inherent complexity of developing and main…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
  - keyword/safety
---

# PAIChecker: Uncovering and Checking PR-Issue Misalignment in SWE-Bench-Like Benchmarks

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.28587v1)
- published:: 2026-07-30
- updated:: 2026-07-30
- arxiv_id:: 2607.28587v1
- pdf:: https://arxiv.org/pdf/2607.28587v1
- categories:: cs.SE, cs.AI

## Abstract / Summary
SWE-bench-like benchmarks are widely used for evaluating LLM's issue resolution capability. They typically follow a common construction pipeline: each PR (Pull Request) is paired with its linked issue by extracting issue references from the PR description; the issue description is used as the problem statement, and the PR patch serves as the test oracle. However, due to the inherent complexity of developing and maintaining large repositories, such PR-Issue pairings are often misaligned in practice. In this work, we systematically study SWE-bench Verified instances, finding that 13.6% exhibit misalignment across five patterns in eleven fine-grained scenarios. To enable reliable and scalable construction of those benchmarks in the future, we propose PAIChecker, a multi-agent system for checking PR-Issue misalignment in SWE-bench-like benchmarks. Specifically, PAIChecker adopts a three-phase design that combines specific pattern identification, cross-agent label synthesis, and code-level validation, thereby enabling more accurate, generalizable, and progressively verified detection. Experiments on SWE-Gym and SWE-bench Multilingual show that PAIchecker achieves the best performance across all four LLM backbones, reaching up to 92.12% and 91.67% binary accuracy, respectively.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.28587v1)
- [PDF](https://arxiv.org/pdf/2607.28587v1)
- [SWE-ABS: Adversarial Benchmark Strengthening Exposes Inflated Success Rates on Test-based Benchmark](https://arxiv.org/abs/2603.00520) (2026, citations: 9)
- [SWE-Universe: Scale Real-World Verifiable Environments to Millions](https://arxiv.org/abs/2602.02361) (2026, citations: 7)
- [SWE-Lego: Pushing the Limits of Supervised Fine-tuning for Software Issue Resolving](https://arxiv.org/abs/2601.01426) (2026, citations: 25)
- [SWE-EVO: Benchmarking Coding Agents in Long-Horizon Software Evolution Scenarios](https://arxiv.org/abs/2512.18470) (2025, citations: 27)
- [SWE-Bench++: A Framework for the Scalable Generation of Software Engineering Benchmarks from Open-Source Repositories](https://arxiv.org/abs/2512.17419) (2025, citations: 20)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/safety
