---
title: "SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineering Agents"
source: "https://arxiv.org/html/2609.04167v1"
author: "Xin He, Yanlin Wang, Mingwei Liu, Jiachi Chen, Hongyu Zhang, Guanbin Li"
published: "2026-09-03"
created: 2026-09-06
description: "Repository-level software engineering benchmarks have significantly advanced the evaluation of coding agents, but existing benchmarks primarily measure whether generated patches pass functional tests and overlook review-derived acceptance constraints (review constraints) that often influence whether a patch is acceptable in real-world software development. We introduce SWE-Gate, a repository-level benchmark for soft…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
---

# SWE-Gate: Passing Functional Tests Is Not Enough for Software Engineering Agents

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.04167v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.04167v1
- pdf:: https://arxiv.org/pdf/2609.04167v1
- categories:: cs.SE, cs.AI

## Abstract / Summary
Repository-level software engineering benchmarks have significantly advanced the evaluation of coding agents, but existing benchmarks primarily measure whether generated patches pass functional tests and overlook review-derived acceptance constraints (review constraints) that often influence whether a patch is acceptable in real-world software development. We introduce SWE-Gate, a repository-level benchmark for software engineering agents that explicitly evaluates review constraint compliance alongside functional correctness. SWE-Gate derives review constraints from real pull request review comments and synthesizes repository-level repair instances around these constraints. Each instance provides separate functional and constraint tests, together with non-compliant and gold patches, enabling explicit separation between issue resolution capability and review constraint compliance. We construct SWE-Gate with 303 repository-level repair instances spanning 75 open-source Python repositories across diverse software domains. Experiments with four LLM backends spanning different capability levels under a common coding-agent scaffold reveal a substantial gap between functional success and success under the complete repair specification: among 644 repairs that pass the functional tests, 221 fail to satisfy the provided review constraints. These findings show that functional-only evaluation overestimates agents' ability to satisfy the full requirements of repository-level repair tasks. The replication package including code, data, and experimental results is available at https://github.com/DeepSoftwareAnalytics/SWE-Gate.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.04167v1)
- [PDF](https://arxiv.org/pdf/2609.04167v1)
- [RepoReasoner: Evaluating Repository-Level Code Reasoning Ability of Long-Context Language Models](https://arxiv.org/abs/2607.25996) (2026, citations: 5)
- [Does Pass Rate Tell the Whole Story? Evaluating Design Constraint Compliance in LLM-based Issue Resolution](https://arxiv.org/abs/2604.05955) (2026, citations: 3)
- [RealSec-bench: A Benchmark for Evaluating Secure Code Generation in Real-World Repositories](https://arxiv.org/abs/2601.22706) (2026, citations: 13)
- [Knowledge Matters: Injecting Project and Testing Knowledge into LLM-based Unit Test Generation](https://arxiv.org/abs/2511.14224) (2025, citations: 4)
- [AlignCoder: Aligning Retrieval with Target Intent for Repository-Level Code Completion](https://arxiv.org/abs/2601.19697) (2025, citations: 9)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/evaluation #keyword/benchmark #keyword/agents
