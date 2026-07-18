---
title: "SearchOS-V1: Towards Robust Open-Domain Information-Seeking Agent Collaboration"
source: "https://arxiv.org/html/2607.15257v1"
author: "Yuyao Zhang, Junjie Gao, Zhengxian Wu, Jiaming Fan, Jin Zhang, Shihan Ma, Yao Yao, Weiran Qi, Chuyan Jin, Guiyu Ma, Xingzhong Xu, Kai Yang, Ji-Rong Wen, Zhicheng Dou"
published: "2026-07-16"
created: 2026-07-19
description: "Multi-agent search system with explicit shared state (SOCM: Frontier Task, Evidence Graph, Coverage Map, Failure Memory), pipeline-parallel scheduling, and tool middleware. Leads WideSearch/GISA."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/agents
  - keyword/retrieval
  - keyword/language-model
  - keyword/reasoning
---

# SearchOS-V1: Towards Robust Open-Domain Information-Seeking Agent Collaboration

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15257v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15257v1
- pdf:: https://arxiv.org/pdf/2607.15257v1
- categories:: cs.AI, cs.CL, cs.IR

## Abstract / Summary
Tool-integrated LLMs make web search core to information-seeking agents, but long histories cause lost progress and repetitive failed-search loops that waste budget. SearchOS turns fragile implicit progress into explicit, persistent, shared state. Open-domain seeking is cast as relational schema completion with grounded citations. Search-Oriented Context Management (SOCM) externalizes Frontier Task, Evidence Graph, Coverage Map, and Failure Memory. Pipeline-parallel scheduling overlaps sub-agents and refills slots toward unresolved coverage gaps. A Search Tool Middleware Harness intercepts model/tool interactions to record evidence and react to stalls/budget exhaustion, plus hierarchical strategy/access skills. On WideSearch and GISA, SearchOS leads evaluated single- and multi-agent baselines. Code: https://github.com/antins-labs/SearchOS

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15257v1)
- [PDF](https://arxiv.org/pdf/2607.15257v1)
- [Code](https://github.com/antins-labs/SearchOS)
- [Code as Agent Harness](https://arxiv.org/abs/2605.18747) (2026, citations: 9)
- [Web2BigTable](https://arxiv.org/abs/2604.27221) (2026, citations: 2)
- [GISA](https://arxiv.org/abs/2602.08543) (2026, citations: 4)
- [Table-as-Search](https://arxiv.org/abs/2602.06724) (2026, citations: 3)
- [A-MapReduce](https://arxiv.org/abs/2602.01331) (2026, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/agents #keyword/retrieval #keyword/language-model #keyword/reasoning
