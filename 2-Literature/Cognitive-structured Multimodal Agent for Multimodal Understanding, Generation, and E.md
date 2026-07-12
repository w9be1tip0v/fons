---
title: "Cognitive-structured Multimodal Agent for Multimodal Understanding, Generation, and Editing"
source: "https://arxiv.org/html/2607.08497v1"
author: "Feng Wang, Canmiao Fu, Zhipeng Huang, Chen Li, Jing Lyu, Ge Li"
published: "2026-07-09"
created: 2026-07-13
description: "Recent unified multimodal models show a single architecture can jointly perform vision/language understanding and image generation/editing. However, they repeatedly feed all historical visual and textual inputs into a shared context window, limiting long-horizon multimodal dialogue due to visual token explosion and unreliable cross-turn referencing. We propose a Cognitive-structured Multimodal Agent that externalizes visual information into an Episodic Visual Memory and selectively reactivates relevant episodes during reasoning."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/multimodal
  - keyword/agents
  - keyword/language-model
  - keyword/nlp
  - keyword/reasoning
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
---

# Cognitive-structured Multimodal Agent for Multimodal Understanding, Generation, and Editing

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.08497v1)
- published:: 2026-07-09
- updated:: 2026-07-09
- arxiv_id:: 2607.08497v1
- pdf:: https://arxiv.org/pdf/2607.08497v1
- categories:: cs.CV, cs.AI, cs.CL, cs.LG

## Abstract / Summary
Recent unified multimodal models show a single architecture can jointly perform vision/language understanding and image generation/editing. However, they repeatedly feed all historical visual and textual inputs into a shared context window, limiting long-horizon multimodal dialogue due to visual token explosion and unreliable cross-turn referencing. We propose a Cognitive-structured Multimodal Agent that externalizes visual information into an Episodic Visual Memory and selectively reactivates relevant episodes during reasoning. The agent consists of a Perceptual Abstraction Engine for structured visual abstraction, a Cognitive Retrieval Engine for cross-turn memory retrieval, and a Multimodal Executive Controller for autonomous task inference and action planning. To address the lack of turn-level retrieval supervision in existing datasets, we develop a Unified Scenario Engine that programmatically generates structured multi-turn conversations with fine-grained retrieval annotations, enabling reinforcement learning to optimize abstraction and retrieval policies. We also construct a long-horizon visual-dialogue benchmark stratified by difficulty to evaluate episodic visual recall. Our 8B agent achieves 91.4% retrieval accuracy over 20-turn sessions, surpassing 32B baselines by +8.2% while nearly halving per-turn inference time (23.1s -> 12.7s). We further present the Cognitive-structured Multimodal Agent Harness (CMA-Harness), a tool-augmented deployment of the same cognitive structure integrating persistent multimodal memory, web access, image generation/editing/composition tools, and OpenAI-compatible serving. Structured memory and modular decision-making offer a more scalable, efficient paradigm for long-horizon multimodal agents than monolithic parameter scaling. Code: https://github.com/caseclose/cma-harness ; Project page: https://caseclose.github.io/cma-harness/

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.08497v1)
- [PDF](https://arxiv.org/pdf/2607.08497v1)
- [Project page](https://caseclose.github.io/cma-harness/)
- [Code](https://github.com/caseclose/cma-harness)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/multimodal #keyword/agents #keyword/language-model #keyword/nlp #keyword/reasoning #keyword/retrieval #keyword/evaluation #keyword/benchmark
