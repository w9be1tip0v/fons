---
title: "Learning User Simulators with Turing Rewards"
source: "https://arxiv.org/html/2606.19336v1"
author: "Yingshan Susan Wang, Cedegao E. Zhang, Linlu Qiu, Zexue He, Pengyuan Li, Alex Pentland, Roger P. Levy, Yoon Kim"
published: "2026-06-17"
created: 2026-06-19
description: "Learning to simulate human users in interactive settings could advance the training of agent assistants, evaluation of personalization systems, research in the social sciences, and more. Existing approaches generally do so by training a large language model (LLM) to match a single ground truth response, either by maximizing the log probability or by using a similarity reward. We instead propose {Turing-RL}: a Turing…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/agents
  - keyword/machine-learning
---

# Learning User Simulators with Turing Rewards

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.19336v1)
- published:: 2026-06-17
- updated:: 2026-06-17
- arxiv_id:: 2606.19336v1
- pdf:: https://arxiv.org/pdf/2606.19336v1
- categories:: cs.CL

## Abstract / Summary
Learning to simulate human users in interactive settings could advance the training of agent assistants, evaluation of personalization systems, research in the social sciences, and more. Existing approaches generally do so by training a large language model (LLM) to match a single ground truth response, either by maximizing the log probability or by using a similarity reward. We instead propose {Turing-RL}: a Turing-Test-based reinforcement learning approach for training user simulator models. {Turing-RL} uses a discriminative Turing reward with an LLM judge to score how indistinguishable a generated response is from the real user's given the user's history, and the user simulator LLM learns to produce responses indistinguishable from what the user could have said with such rewards. Across two different domains--conversational chat and Reddit forum discussion--we find that {Turing-RL} consistently outperforms baseline methods on both LLM and human evaluation metrics. Our study suggests that optimizing for indistinguishability, rather than response matching, is effective for learning user simulators.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.19336v1)
- [PDF](https://arxiv.org/pdf/2606.19336v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/agents #keyword/machine-learning
