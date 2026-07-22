---
title: "Inference-Time Steering for Cross-Lingual Factual Consistency in LLMs"
source: "https://arxiv.org/html/2607.19243v1"
author: "Alexander Manev"
published: "2026-07-21"
created: 2026-07-23
description: "Although Large Language Models (LLMs) demonstrate remarkable multilingual fluency, their internal knowledge representations remain disproportionately biased toward high-resource languages. This leads to cross-lingual factual inconsistency, where they shift their empirical answer distributions based solely on the prompt language. We investigate whether these biases can be mitigated at inference time, forcing an Engli…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/safety
  - keyword/machine-learning
---

# Inference-Time Steering for Cross-Lingual Factual Consistency in LLMs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.19243v1)
- published:: 2026-07-21
- updated:: 2026-07-21
- arxiv_id:: 2607.19243v1
- pdf:: https://arxiv.org/pdf/2607.19243v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Although Large Language Models (LLMs) demonstrate remarkable multilingual fluency, their internal knowledge representations remain disproportionately biased toward high-resource languages. This leads to cross-lingual factual inconsistency, where they shift their empirical answer distributions based solely on the prompt language. We investigate whether these biases can be mitigated at inference time, forcing an English-prompted model to answer as if it were queried in target languages (German, Spanish, Bulgarian), and evaluate four intervention strategies: zero-shot contextual steering (persona prompting), internal representation manipulation via Contrastive Activation Addition (CAA), and lightweight weight modification via Direct Preference Optimization (DPO) trained on benchmark-derived factual data as well as conceptual generalization data. To assess alignment, we curate a multilingual factual dataset alongside a novel generalization benchmark comprising culturally rooted queries to determine whether factual interventions transfer to broader target-centric preferences. Experiments on Gemma 3 12B Instruct reveal persona prompting to be the strongest overall intervention, balancing efficacy, safety, and out-of-domain generalization. While CAA yields sharp inconsistency benchmark shifts, it is configuration-sensitive and risks knowledge degradation. DPO-based adapters offer permanent, yet narrower and less transferable gains. These findings suggest that cross-lingual inconsistency is at least partly a selection problem, and that simple contextual interventions may outperform more invasive methods for robust, transferable alignment.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.19243v1)
- [PDF](https://arxiv.org/pdf/2607.19243v1)
- [AlignX: Advancing Multilingual Large Language Models with Multilingual Representation Alignment](https://arxiv.org/abs/2509.24338) (2025, citations: 8)
- [Aligning LLMs for Multilingual Consistency in Enterprise Applications](https://arxiv.org/abs/2509.23659) (2025, citations: 13)
- [The Prompt Makes the Person(a): A Systematic Evaluation of Sociodemographic Persona Prompting for Large Language Models](https://arxiv.org/abs/2507.16076) (2025, citations: 32)
- [Multilingual Prompting for Improving LLM Generation Diversity](https://arxiv.org/abs/2505.15229) (2025, citations: 18)
- [From Unaligned to Aligned: Scaling Multilingual LLMs with Multi-Way Parallel Corpora](https://arxiv.org/abs/2505.14045) (2025, citations: 7)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/safety #keyword/machine-learning
