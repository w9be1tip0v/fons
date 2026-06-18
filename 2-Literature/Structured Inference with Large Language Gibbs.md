---
title: "Structured Inference with Large Language Gibbs"
source: "https://arxiv.org/html/2606.19264v1"
author: "Sanghyeok Choi, Henry Gouk, Esmeralda S. Whitammer"
published: "2026-06-17"
created: 2026-06-19
description: "The knowledge encoded in large language models (LLMs) can serve as a substrate for structured reasoning over variables describing a complex world, but accessing this knowledge in a probabilistically coherent manner poses a difficult inference problem. We propose Large Language Gibbs, a scheme for structured probabilistic inference that uses conditional distributions of an LLM as transition operators. Rather than sam…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/reasoning
  - keyword/machine-learning
---

# Structured Inference with Large Language Gibbs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.19264v1)
- published:: 2026-06-17
- updated:: 2026-06-17
- arxiv_id:: 2606.19264v1
- pdf:: https://arxiv.org/pdf/2606.19264v1
- categories:: cs.LG, cs.CL

## Abstract / Summary
The knowledge encoded in large language models (LLMs) can serve as a substrate for structured reasoning over variables describing a complex world, but accessing this knowledge in a probabilistically coherent manner poses a difficult inference problem. We propose Large Language Gibbs, a scheme for structured probabilistic inference that uses conditional distributions of an LLM as transition operators. Rather than sampling structured objects through single-pass autoregressive generation, we iteratively resample individual variables conditioned on others using an LLM's next-token conditionals. This approach avoids order-dependent biases and produces a stationary distribution that reflects a compromise between all local conditionals. We apply this approach to sampling from synthetic distributions, consistent reasoning tasks, and Bayesian structure learning. The results suggest that the use of LLM conditionals in MCMC is a practical alternative to one-pass generation for structured probabilistic inference under a world prior accessible through noisy LLM conditionals.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.19264v1)
- [PDF](https://arxiv.org/pdf/2606.19264v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/reasoning #keyword/machine-learning
