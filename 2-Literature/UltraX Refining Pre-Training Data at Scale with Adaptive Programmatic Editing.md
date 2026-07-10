---
title: "UltraX: Refining Pre-Training Data at Scale with Adaptive Programmatic Editing"
source: "https://arxiv.org/html/2607.08646v1"
author: "Xinlong Zhao, Dongsheng Liu, Hengyu Zhao, Zixuan Fu, Zheng Wang, Jie Cai, Jie Zhou, Qiang Ma, Xuanhe Zhou, Xu Han, Yudong Wang, Zhiyuan Liu"
published: "2026-07-09"
created: 2026-07-11
description: "As available training data approaches its physical limit, gains from Scaling Laws have begun to diminish. Consequently, improving Large Language Models (LLMs) now depends less on data expansion and more on higher-quality data utilization. However, in the context of large-scale corpora, existing refinement methodologies face significant limitations in quality, efficiency, and reliability: Rule-based approaches are co…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/safety
  - keyword/machine-learning
---

# UltraX: Refining Pre-Training Data at Scale with Adaptive Programmatic Editing

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.08646v1)
- published:: 2026-07-09
- updated:: 2026-07-09
- arxiv_id:: 2607.08646v1
- pdf:: https://arxiv.org/pdf/2607.08646v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
As available training data approaches its physical limit, gains from Scaling Laws have begun to diminish. Consequently, improving Large Language Models (LLMs) now depends less on data expansion and more on higher-quality data utilization. However, in the context of large-scale corpora, existing refinement methodologies face significant limitations in quality, efficiency, and reliability: Rule-based approaches are constrained by fixed heuristics and struggle with instance-level variations; LLM-based approaches improve quality but fail to meet the efficiency and reliability requirements of large-scale data processing. To address these challenges, we propose UltraX, a function-calling refinement framework for large-scale pre-training data that completes the editing function space by introducing insertion in addition to deletion and modification, enabling fine-grained instance-level editing. Specifically, UltraX builds a reliable program-supervision generation pipeline. In this pipeline, dataset-adaptive prompt optimization first guides an expert LLM to produce high-quality end-to-end refined texts, and Line Alignment Mapping and Dynamic Context Replacement then convert original-refined text pairs into structured program supervision. Meanwhile, UltraX improves supervision quality and stabilizes the training distribution with low-confidence example filtering and ratio-controlled sampling by operation combination. During inference and execution, it normalizes and validates model outputs through sliding-window prediction, global operation aggregation, and systematic post-processing, improving the stability and reliability of large-scale execution. Experiments show that UltraX achieves the highest average performance across all corpora and also matches or surpasses baselines w…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.08646v1)
- [PDF](https://arxiv.org/pdf/2607.08646v1)
- [DeepSeek-V4: Towards Highly Efficient Million-Token Context Intelligence](https://arxiv.org/abs/2606.19348) (2026, citations: 262)
- [Data Science and Technology Towards AGI Part I: Tiered Data Management](https://arxiv.org/abs/2602.09003) (2026, citations: 1)
- [DeepSeek-V3.2: Pushing the Frontier of Open Large Language Models](https://arxiv.org/abs/2512.02556) (2025, citations: 617)
- [AICC: Parse HTML Finer, Make Models Better - A 7.3T AI-Ready Corpus Built by a Model-Based HTML Parser](https://arxiv.org/abs/2511.16397) (2025, citations: 2)
- [Gemini 2.5: Pushing the Frontier with Advanced Reasoning, Multimodality, Long Context, and Next Generation Agentic Capabilities](https://arxiv.org/abs/2507.06261) (2025, citations: 3514)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/safety #keyword/machine-learning
