---
title: "Prefix Sliding for efficient test-time scaling"
source: "https://arxiv.org/html/2608.26070v1"
author: "Niklas Muennighoff, Zhengyang Wang, Zeyi Chen, Weijia Shi, Binyuan Hui, John Yang, Dapeng Jiang, Mika Senghaas, Fares Obeid, Johannes Hagemann, Sami Jaghouar, Ludwig Schmidt, Percy Liang, Jason Wei, Andrew Y. Ng, Luke Zettlemoyer, Yejin Choi, Mike Lewis"
published: "2026-08-26"
created: 2026-08-28
description: "Test-time scaling uses extra test-time compute to improve performance, such as letting language models reason longer when solving a problem. As models keep the entire reasoning trace in memory via full attention, hard tasks that need long thinking can be prohibitively expensive. However, we find most intermediate reasoning tokens lose importance as the model continues reasoning. This calls into question whether reta…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/transformer
  - keyword/language-model
  - keyword/nlp
  - keyword/reasoning
  - keyword/agents
  - keyword/machine-learning
---

# Prefix Sliding for efficient test-time scaling

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.26070v1)
- published:: 2026-08-26
- updated:: 2026-08-26
- arxiv_id:: 2608.26070v1
- pdf:: https://arxiv.org/pdf/2608.26070v1
- categories:: cs.CL, cs.AI, cs.LG

## Abstract / Summary
Test-time scaling uses extra test-time compute to improve performance, such as letting language models reason longer when solving a problem. As models keep the entire reasoning trace in memory via full attention, hard tasks that need long thinking can be prohibitively expensive. However, we find most intermediate reasoning tokens lose importance as the model continues reasoning. This calls into question whether retaining them is worth the cost. Based on this insight, we propose Prefix Sliding, which discards tokens during reasoning that are not part of the prefix or the window of the last few thousand tokens. The prefix has key instructions and tools available to the model, while the most recent tokens are the current reasoning the model is working on. This caps the total memory requirement regardless of how long the model reasons, allowing for efficient long-horizon test-time scaling. Without training, Prefix Sliding can make existing models 3x faster while maintaining performance. Training with Prefix Sliding using reinforcement learning can achieve better performance by enabling scaling to reasoning traces beyond a hundred thousand tokens. Ablations show Prefix Sliding outperforms summarizing intermediate tokens or vanilla sliding window. Our code is at https://github.com/Muennighoff/prefix-sliding

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.26070v1)
- [PDF](https://arxiv.org/pdf/2608.26070v1)
- [Lost in Compaction: Evaluating Side-Constraint Loss under Context Compaction](https://arxiv.org/abs/2608.11242) (2026, citations: 1)
- [Self-Compacting Language Model Agents](https://arxiv.org/abs/2606.23525) (2026, citations: 1)
- [Sparrow: Sparse Rollout for Stable and Efficient Long-context RL of Large Language Models](https://arxiv.org/abs/2606.08446) (2026, citations: 1)
- [Value-Aware Stochastic KV Cache Eviction for Reasoning Models](https://arxiv.org/abs/2606.03928) (2026, citations: 4)
- [KARA: Efficient Reasoning LLM Serving via Sliding-Window KV Cache Compression](https://arxiv.org/abs/2607.01237) (2026, citations: 1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/transformer #keyword/language-model #keyword/nlp #keyword/reasoning #keyword/agents #keyword/machine-learning
