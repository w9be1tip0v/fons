---
title: "Legibility is Not Interpretability: Comparing Judged and Actual Importance in Chain-Of-Thought Reasoning"
source: "https://arxiv.org/html/2609.04194v1"
author: "Kevin Du, Alexander Hoyle, Laura Ruis, Acyr Locatelli"
published: "2026-09-03"
created: 2026-09-05
description: "Reasoning traces from chain-of-thought models appear to offer a legible window into how a model arrives at its answer. A growing body of work treats them as such, using LLM judges to diagnose errors, evaluate faithfulness, and provide step-level supervision via process reward models and generative critics. These practices rely on the text of a reasoning step carrying information about its functional role. But does t…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/reasoning
  - keyword/machine-learning
---

# Legibility is Not Interpretability: Comparing Judged and Actual Importance in Chain-Of-Thought Reasoning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.04194v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.04194v1
- pdf:: https://arxiv.org/pdf/2609.04194v1
- categories:: cs.CL, cs.LG

## Abstract / Summary
Reasoning traces from chain-of-thought models appear to offer a legible window into how a model arrives at its answer. A growing body of work treats them as such, using LLM judges to diagnose errors, evaluate faithfulness, and provide step-level supervision via process reward models and generative critics. These practices rely on the text of a reasoning step carrying information about its functional role. But does the text actually encode information about which reasoning steps matter? We operationalize the importance of a reasoning step as its advantage: the change in expected reward, e.g., producing the correct final answer, from including that step, estimated via Monte Carlo rollouts. Basing ground truth on these estimates, we evaluate whether LLM judges can identify high-advantage steps and find that sufficiently capable LLMs can outperform a prevalence baseline but fall well short of a noise ceiling. Fine-tuning a model as a step-level critic yields strong improvement for incorrect responses but remains distant from ceiling for correct responses, suggesting that step importance is only partially recoverable from the text of the reasoning trace. Our findings contribute to a growing body of chain-of-thought faithfulness work that cautions against treating the legibility of reasoning traces as interpretability, especially with implications for process reward modeling.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.04194v1)
- [PDF](https://arxiv.org/pdf/2609.04194v1)
- [Reasoning Theater: Disentangling Model Beliefs from Chain-of-Thought](https://arxiv.org/abs/2603.05488) (2026, citations: 32)
- [Towards Long-Horizon Interpretability: Efficient and Faithful Multi-Token Attribution for Reasoning LLMs](https://arxiv.org/abs/2602.01914) (2026, citations: 4)
- [State over Tokens: Characterizing the Role of Reasoning Tokens](https://arxiv.org/abs/2512.12777) (2025, citations: 6)
- [Do LLMs Really Need 10+ Thoughts for "Find the Time 1000 Days Later"? Towards Structural Understanding of LLM Overthinking](https://arxiv.org/abs/2510.07880) (2025, citations: 9)
- [How Persuasive is Your Context?](https://arxiv.org/abs/2509.17879) (2025, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/reasoning #keyword/machine-learning
