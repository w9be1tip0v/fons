---
title: "3D-Aware VLMs with Implicit and Explicit Geometries"
source: "https://arxiv.org/html/2607.21595v1"
author: "Wenhao Li, Xueying Jiang, Quanhao Qian, Deli Zhao, Ran Xu, Shijian Lu, Gongjie Zhang"
published: "2026-07-23"
created: 2026-07-26
description: "Despite rapid progress, most existing vision-language models (VLMs) built from 2D visual inputs often struggle when handling various 3D tasks that require fine-grained spatial understanding and reasoning. To bridge this gap, we present VLM-IE3D, a unified framework that enhances the 3D spatial awareness of VLMs by equipping them with both implicit and explicit 3D geometries learned from RGB videos. Our VLM-IE3D intr…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/reasoning
---

# 3D-Aware VLMs with Implicit and Explicit Geometries

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.21595v1)
- published:: 2026-07-23
- updated:: 2026-07-23
- arxiv_id:: 2607.21595v1
- pdf:: https://arxiv.org/pdf/2607.21595v1
- categories:: cs.CV, cs.AI, cs.LG

## Abstract / Summary
Despite rapid progress, most existing vision-language models (VLMs) built from 2D visual inputs often struggle when handling various 3D tasks that require fine-grained spatial understanding and reasoning. To bridge this gap, we present VLM-IE3D, a unified framework that enhances the 3D spatial awareness of VLMs by equipping them with both implicit and explicit 3D geometries learned from RGB videos. Our VLM-IE3D introduces Implicit Geometry Tokens (IGTs) that capture high-level geometric priors from input videos, as well as complementary Explicit Geometry Tokens (EGTs) that encode detailed geometric structures from reconstructed 3D attributes. On top of that, VLM-IE3D comes with a 3D-aware adapter that effectively fuses the two types of geometric representations with 2D visual cues. This RGB-only design injects strong 3D inductive biases for fine-grained spatial understanding and reasoning without requiring any additional 3D inputs. Extensive experiments show that VLM-IE3D achieves superior performance consistently across various 3D tasks including 3D video detection, 3D visual grounding, 3D dense captioning, and spatial reasoning. Code and models are available at https://github.com/Vegetebird/VLM-IE3D.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.21595v1)
- [PDF](https://arxiv.org/pdf/2607.21595v1)
- [Towards Camera-Robust 3D Localization: Equation-Anchored Tool-Use for MLLMs](https://arxiv.org/abs/2605.19528) (2026, citations: 1)
- [On the Generalization Capacities of MLLMs for Spatial Intelligence](https://arxiv.org/abs/2603.06704) (2026, citations: 8)
- [MLLMs Need 3D-Aware Representation Supervision for Scene Understanding](https://arxiv.org/abs/2506.01946) (2025, citations: 61)
- [Learning from Videos for 3D World: Enhancing MLLMs with 3D Vision Geometry Priors](https://arxiv.org/abs/2505.24625) (2025, citations: 104)
- [AnySplat: Feed-forward 3D Gaussian Splatting from Unconstrained Views](https://arxiv.org/abs/2505.23716) (2025, citations: 223)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/reasoning
