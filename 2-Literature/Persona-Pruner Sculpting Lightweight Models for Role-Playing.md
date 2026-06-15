---
title: "Persona-Pruner: Sculpting Lightweight Models for Role-Playing"
source: "https://arxiv.org/html/2606.14695v1"
author: "Jinsu Kim, Jihoon Tack, Noah Lee, Jongheon Jeong"
published: "2026-06-12"
created: 2026-06-16
description: "Language Models (LMs) have shown remarkable potential as role-playing chatbots, delivering consistent, stylized interactions when given a specification of a character or user persona. However, applying these capabilities to real-world applications (e.g., ecosystems with numerous NPCs interacting simultaneously) exposes a critical inefficiency due to the excessive computational cost. In this paper, we question the ne…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/research-paper
---

# Persona-Pruner: Sculpting Lightweight Models for Role-Playing

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.14695v1)
- published:: 2026-06-12
- updated:: 2026-06-12
- arxiv_id:: 2606.14695v1
- pdf:: https://arxiv.org/pdf/2606.14695v1
- categories:: cs.LG, cs.CL

## Abstract / Summary
Language Models (LMs) have shown remarkable potential as role-playing chatbots, delivering consistent, stylized interactions when given a specification of a character or user persona. However, applying these capabilities to real-world applications (e.g., ecosystems with numerous NPCs interacting simultaneously) exposes a critical inefficiency due to the excessive computational cost. In this paper, we question the necessity of dedicating a full, generalist model to a single persona, hypothesizing that a specific character identity relies on only a fraction of the model's total capacity. We observe that naively pruning LMs often severely degrades the role-playing performance for a specific persona; it does not distinguish between redundant knowledge and essential character traits. We propose Persona-Pruner, a framework that sculpts a lightweight role-playing model by isolating persona-specific sub-networks from a single description. Our experiments consistently show that Persona-Pruner preserves role-playing performance substantially more effectively than existing state-of-the-art LLM pruning techniques, reducing the performance drop from the dense model by up to 93.8% over the strongest baseline on RoleBench in LLM-as-a-judge score, while still maintaining general LLM capabilities. Code is available at https://github.com/jsu-kim/Persona-Pruner.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.14695v1)
- [PDF](https://arxiv.org/pdf/2606.14695v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/research-paper
