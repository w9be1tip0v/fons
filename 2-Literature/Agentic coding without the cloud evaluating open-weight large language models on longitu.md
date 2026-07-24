---
title: "Agentic coding without the cloud: evaluating open-weight large language models on longitudinal data preparation tasks"
source: "https://arxiv.org/html/2607.21482v1"
author: "Mack Nixon, Liam Wright, Yevgeniya Kovalchuk, Alison Fang-Wei Wu, Martin Danka, Andy Boyd, David Bann"
published: "2026-07-23"
created: 2026-07-25
description: "Large language models (LLMs) and agents are now widely used tools in code development, with data typically sent to third-party cloud-based models. Their adoption in research using personal data is constrained by governance requirements that typically prohibit data transmission to external services. Locally deployable open-weight models offer an alternative since sensitive data never leave the local environment. We i…"
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
---

# Agentic coding without the cloud: evaluating open-weight large language models on longitudinal data preparation tasks

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.21482v1)
- published:: 2026-07-23
- updated:: 2026-07-23
- arxiv_id:: 2607.21482v1
- pdf:: https://arxiv.org/pdf/2607.21482v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
Large language models (LLMs) and agents are now widely used tools in code development, with data typically sent to third-party cloud-based models. Their adoption in research using personal data is constrained by governance requirements that typically prohibit data transmission to external services. Locally deployable open-weight models offer an alternative since sensitive data never leave the local environment. We introduce an open-source framework for evaluating the efficacy of AI agents powered by open-weight LLMs on one of the most persistent bottlenecks in research on longitudinal population studies: data preparation. The framework comprises: a curated ground-truth dataset (cleaning scripts preparing six sweeps of data from a British cohort study), task definitions encompassing tasks such as category harmonization and multi-wave merging, and automated routines for evaluating the LLM-produced R code and outputted data. We benchmark LLMs across the (consumer grade) deployment spectrum to assess their efficacy in 20 data preparation tasks (creation of 102 variables). Current state-of-the-art, 31-35B parameter models almost saturated our benchmark ("average task completion" up to 87.9%). The performance of open-weight LLMs running on consumer-grade hardware shows promise of a viable path toward AI-assisted data preparation in governance-restricted research settings. Our framework is publicly available at: https://github.com/UCL-ARC/RRBench.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.21482v1)
- [PDF](https://arxiv.org/pdf/2607.21482v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/agents
