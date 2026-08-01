---
title: "LEDGERMIND: Provenance-Constrained Multimodal Agentic Reasoning with a Structured Evidence Ledger"
source: "https://arxiv.org/html/2607.28374v1"
author: "Enjun Du, Hange Zhou, Chenxu Du, Siyi Liu, Zirong Chen, Ziyu Zheng, Yongqi Zhang"
published: "2026-07-30"
created: 2026-08-02
description: "Multimodal agents for visual question answering increasingly operate as multi-step trajectories that interleave perception, retrieval, and reasoning, yet evaluation still largely reduces to final-answer accuracy. This aggregate signal cannot tell whether a correct answer was reached through grounded evidence, language priors, or accidental error cancellation. We propose to treat a multimodal agent trajectory as a pr…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/agents
---

# LEDGERMIND: Provenance-Constrained Multimodal Agentic Reasoning with a Structured Evidence Ledger

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.28374v1)
- published:: 2026-07-30
- updated:: 2026-07-30
- arxiv_id:: 2607.28374v1
- pdf:: https://arxiv.org/pdf/2607.28374v1
- categories:: cs.LG

## Abstract / Summary
Multimodal agents for visual question answering increasingly operate as multi-step trajectories that interleave perception, retrieval, and reasoning, yet evaluation still largely reduces to final-answer accuracy. This aggregate signal cannot tell whether a correct answer was reached through grounded evidence, language priors, or accidental error cancellation. We propose to treat a multimodal agent trajectory as a provenance-constrained state machine: tool outputs are normalized into a Structured Evidence Ledger that serves as the trajectory state, downstream reasoning and decision claims may cite only active ledger entries, grounding is checked at the entity and numeric level, and repair is realized as typed state transitions that cannot introduce content without tool-produced provenance. We instantiate this design as LedgerMind (Provenance-Constrained Multimodal Agentic Reasoning with a Structured Evidence Ledger), augmented by a Three-Layer Grounding Protocol, an Adaptive Dual-Path Dispatcher that matches reasoning depth to question complexity, and an Event-Triggered Verification-and-Repair engine with a formal provenance non-amplification guarantee. We use LedgerMind to target four recurring failure patterns that final-answer accuracy tends to obscure: unsupported intermediate reasoning, citation-backed entity hallucination (Phantom Grounding), over-reasoning on simple queries, and repair-time amplification. Experiments across multiple multimodal reasoning benchmarks and backbone MLLMs show that LedgerMind improves both answer accuracy and trajectory-level faithfulness.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.28374v1)
- [PDF](https://arxiv.org/pdf/2607.28374v1)
- [Claim-Level Rubric Rewards for Video Caption Reinforcement Learning](https://arxiv.org/abs/2607.05150) (2026, citations: 2)
- [VTC-Bench: Evaluating Agentic Multimodal Models via Compositional Visual Tool Chaining](https://arxiv.org/abs/2603.15030) (2026, citations: 7)
- [MC-Search: Evaluating and Enhancing Multimodal Agentic Search with Structured Long Reasoning Chains](https://arxiv.org/abs/2603.00873) (2026, citations: 8)
- [VideoSeg-R1:Reasoning Video Object Segmentation via Reinforcement Learning](https://arxiv.org/abs/2511.16077) (2025, citations: 6)
- [Octopus: Agentic Multimodal Reasoning with Six-Capability Orchestration](https://arxiv.org/abs/2511.15351) (2025, citations: 8)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/agents
