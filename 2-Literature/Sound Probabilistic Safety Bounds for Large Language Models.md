---
title: "Sound Probabilistic Safety Bounds for Large Language Models"
source: "https://arxiv.org/html/2607.20286v1"
author: "Mahdi Nazeri, Anne-Kathrin Schmuck, Sadegh Soudjani, Alessandro Abate"
published: "2026-07-22"
created: 2026-07-24
description: "We propose a novel framework for computing rigorous bounds on the probability that a large language model (LLM) generates harmful output to a given prompt. We study a new application of the Clopper-Pearson confidence intervals to obtain probably approximately correct (PAC) bounds for this problem. As our main technical contribution, we propose an algorithm that leverages features in the latent space to prioritize ex…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/safety
---

# Sound Probabilistic Safety Bounds for Large Language Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.20286v1)
- published:: 2026-07-22
- updated:: 2026-07-22
- arxiv_id:: 2607.20286v1
- pdf:: https://arxiv.org/pdf/2607.20286v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
We propose a novel framework for computing rigorous bounds on the probability that a large language model (LLM) generates harmful output to a given prompt. We study a new application of the Clopper-Pearson confidence intervals to obtain probably approximately correct (PAC) bounds for this problem. As our main technical contribution, we propose an algorithm that leverages features in the latent space to prioritize exploring branches in the auto-regressive generation tree that are more likely to produce harmful outputs. Our approach in particular enables the efficient computation of useful lower bounds, even in scenarios where the true harm probability is extremely small, and crucially, the obtained lower bounds are sound, i.e., formally proven to be less than the actual harmfulness probability: our experimental results demonstrate the effectiveness of our method by computing non-trivial lower bounds on state-of-the-art LLMs. This study newly enables the evaluation and statistical certification of LLMs.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.20286v1)
- [PDF](https://arxiv.org/pdf/2607.20286v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/safety
