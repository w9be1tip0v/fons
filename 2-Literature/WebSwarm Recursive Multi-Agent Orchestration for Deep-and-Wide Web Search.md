---
title: "WebSwarm: Recursive Multi-Agent Orchestration for Deep-and-Wide Web Search"
source: "https://arxiv.org/html/2607.08662v1"
author: "Xiaoshuai Song, Liancheng Zhang, Kangzhi Zhao, Yutao Zhu, Zhongyuan Wang, Guanting Dong, Jinghan Yang, Han Li, Kun Gai, Ji-Rong Wen, Zhicheng Dou"
published: "2026-07-09"
created: 2026-07-11
description: "Large language model (LLM)-based web search agents are transforming information seeking from simple factoid question answering into complex, deep-and-wide search and research-oriented tasks. A single ReAct-style agent is constrained by one long trajectory and limited context, making it difficult to handle depth and coverage simultaneously. Existing multi-agent systems improve search coverage through parallel executi…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/agents
  - keyword/machine-learning
---

# WebSwarm: Recursive Multi-Agent Orchestration for Deep-and-Wide Web Search

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.08662v1)
- published:: 2026-07-09
- updated:: 2026-07-09
- arxiv_id:: 2607.08662v1
- pdf:: https://arxiv.org/pdf/2607.08662v1
- categories:: cs.CL, cs.AI, cs.MA

## Abstract / Summary
Large language model (LLM)-based web search agents are transforming information seeking from simple factoid question answering into complex, deep-and-wide search and research-oriented tasks. A single ReAct-style agent is constrained by one long trajectory and limited context, making it difficult to handle depth and coverage simultaneously. Existing multi-agent systems improve search coverage through parallel execution and aggregation, but still exhibit clear limitations in recursive depth, collaboration adaptability, and evidence-grounded expansion. We propose WebSwarm, a progressive recursive delegation framework that jointly constructs task decomposition, recursive expansion, and agent collaboration during inference. WebSwarm dynamically instantiates agentic search nodes, each coupling a local objective with a search mode that specifies how the node should organize search and collaboration. Each node can either solve its objective itself or further delegate child nodes; after solving, it returns evidence and results upward, enabling parent nodes to further expand, revise, or aggregate the search process. To guide this process, WebSwarm first probes how task-relevant information is organized on the web to ground subsequent node expansion, and reuses process-level experience across homogeneous sibling nodes. Experiments on BrowseComp-Plus, WideSearch, DeepWideSearch, and GISA show that WebSwarm consistently outperforms single-agent and multi-agent baselines on deep, wide, and interleaved deep-and-wide tasks. Further analyses of ablation, task difficulty, web tool efficiency, and model generalization explain WebSwarm's effectiveness and provide insights for multi-agent search systems.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.08662v1)
- [PDF](https://arxiv.org/pdf/2607.08662v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/agents #keyword/machine-learning
