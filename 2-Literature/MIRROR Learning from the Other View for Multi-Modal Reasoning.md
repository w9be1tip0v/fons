---
title: "MIRROR: Learning from the Other View for Multi-Modal Reasoning"
source: "https://arxiv.org/html/2607.21552v1"
author: "Wen Ye, Yuxiao Qu, Aviral Kumar, Xuezhe Ma"
published: "2026-07-23"
created: 2026-07-26
description: "Unlike large language models (LLMs) that exhibit strong reasoning capabilities, vision-language models (VLMs) struggle with visual reasoning, even on geometry problems that admit equivalent text, diagram, and combined diagram+text views. We show that these views often elicit different behaviors: a model may solve a problem from text but fail on the corresponding diagram, or succeed visually while failing textually.…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/machine-learning
---

# MIRROR: Learning from the Other View for Multi-Modal Reasoning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.21552v1)
- published:: 2026-07-23
- updated:: 2026-07-23
- arxiv_id:: 2607.21552v1
- pdf:: https://arxiv.org/pdf/2607.21552v1
- categories:: cs.AI, cs.LG

## Abstract / Summary
Unlike large language models (LLMs) that exhibit strong reasoning capabilities, vision-language models (VLMs) struggle with visual reasoning, even on geometry problems that admit equivalent text, diagram, and combined diagram+text views. We show that these views often elicit different behaviors: a model may solve a problem from text but fail on the corresponding diagram, or succeed visually while failing textually. This inconsistency suggests that different views expose complementary reasoning paths and failure modes that standard multimodal post-training does not fully exploit. To study and exploit this phenomenon, we construct ODA-Data, a high-quality paired multimodal geometry dataset with text-dominant, image-dominant, and combined image+text views of the same problems, together with splits for training and evaluating modality-dependent reasoning behaviors. We then develop Modality-Informed Reciprocal Reasoning Optimization (MIRROR), a reinforcement learning approach for improving multimodal reasoning via self supervision. For each problem, MIRROR evaluates the model under all views, selects the best-performing view as a teacher, and trains other views with a reverse-KL objective towards the teacher. Across reasoning benchmarks that evaluate on geometry problems, MIRROR improves over standard RL and yields more accurate and consistent behavior across modalities

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.21552v1)
- [PDF](https://arxiv.org/pdf/2607.21552v1)
- [UnityMAS-O: A General RL Optimization Framework for LLM-Based Multi-Agent Systems](https://arxiv.org/abs/2605.26646) (2026, citations: 2)
- [Act2See: Emergent Active Visual Perception for Video Reasoning](https://arxiv.org/abs/2605.01657) (2026, citations: 1)
- [MAD-OPD: Breaking the Ceiling in On-Policy Distillation via Multi-Agent Debate](https://arxiv.org/abs/2605.01347) (2026, citations: 4)
- [Do Vision-Language Models Truly Perform Vision Reasoning? A Rigorous Study of the Modality Gap](https://arxiv.org/abs/2604.16256) (2026, citations: 2)
- [Rethinking On-Policy Distillation of Large Language Models: Phenomenology, Mechanism, and Recipe](https://arxiv.org/abs/2604.13016) (2026, citations: 121)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/machine-learning
