---
title: "S3Gym: Can LLMs Turn Self-Testing and Self-Judging into Self-Improvement?"
source: "https://arxiv.org/html/2608.31100v1"
author: "Jiajun Shi, Siyuan Tao, Yuhao Wu, Zexuan Wang, Jingyuan Zhang, Jiaheng Liu, Xinping Lei, Xinrong Zhang, Siyuan Fang, Zhewen Tan, Tianle Cai, Junhao Fang, Jiameng Huang, Yueyang Wang, Jinkai Liu, Yuxuan Zhang, Jian Yang, Zhoujun Li, Shen Yan, Wenhao Huang, Ge Zhang"
published: "2026-08-31"
created: 2026-09-02
description: "Large language models (LLMs) increasingly interact with external environments and accumulate substantial behavioral experience, yet existing agent benchmarks largely evaluate them as fixed policies. It therefore remains unclear whether an agent can actively test its behavior, judge the resulting experience, and use that experience to improve future decisions. We introduce \textbf{S\textsuperscript{3}Gym}, an interac…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
  - keyword/machine-learning
---

# S3Gym: Can LLMs Turn Self-Testing and Self-Judging into Self-Improvement?

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.31100v1)
- published:: 2026-08-31
- updated:: 2026-08-31
- arxiv_id:: 2608.31100v1
- pdf:: https://arxiv.org/pdf/2608.31100v1
- categories:: cs.CL

## Abstract / Summary
Large language models (LLMs) increasingly interact with external environments and accumulate substantial behavioral experience, yet existing agent benchmarks largely evaluate them as fixed policies. It therefore remains unclear whether an agent can actively test its behavior, judge the resulting experience, and use that experience to improve future decisions. We introduce \textbf{S\textsuperscript{3}Gym}, an interactive benchmark for evaluating LLM self-improvement through three coupled capabilities: \textbf{Self-Testing}, \textbf{Self-Judging}, and \textbf{Self-Improvement}. S$^3$Gym separates permissive exploration from strict held-out evaluation and instantiates this protocol in seven text-based games with executable environment verifiers. We evaluate three pathways for incorporating interaction experience: direct History ICL, score-conditioned Summary Memory, and parameter Training. Our experiments reveal that self-improvement is neither automatic nor uniform. Context-level experience improves performance for several model--game pairs, but the most effective pathway depends strongly on the task structure: summaries are beneficial when experience can be compressed into reusable strategic rules, yet often underperform raw history when success depends on precise, state-contingent information. Parameter training produces substantial gains on some tasks, but also exhibits unstable improvement and severe negative transfer on others. These findings show that recognizing successful actions is insufficient; agents must also transform feedback into executable and transferable policies. S$^3$Gym provides a unified framework for diagnosing this process and identifying the bottlenecks that prevent agents from translating interaction experience into reliable self-improvement.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.31100v1)
- [PDF](https://arxiv.org/pdf/2608.31100v1)
- [Credit Without Ground Truth: Auditing Step-Level Credit Assignment in LLM Agents Against Executed Replay](https://arxiv.org/abs/2608.19760) (2026, citations: 2)
- [AI4AI-Bench: Benchmarking LLM Agents in Algorithmic Design for Recursive Self-Improvement](https://arxiv.org/abs/2608.20318) (2026, citations: 2)
- [On the Fragility of Self-Improving Agents: Variance, Task Order, and Underspecification](https://arxiv.org/abs/2608.18066) (2026, citations: 1)
- [Social Gym and SPaRTan: Benchmarking and Improving LLM Social Reasoning via Multi-Agent Game Tournaments](https://arxiv.org/abs/2608.09128) (2026, citations: 1)
- [When Self-Evolution Backfires: Pre-Commit Gating against Skill Contamination in LLM Agents](https://arxiv.org/abs/2608.05810) (2026, citations: 1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/machine-learning
