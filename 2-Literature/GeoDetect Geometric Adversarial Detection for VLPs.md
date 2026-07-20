---
title: "GeoDetect: Geometric Adversarial Detection for VLPs"
source: "https://arxiv.org/html/2607.14737v1"
author: "Afsaneh Hasanebrahimi, Hanxun Huang, Christopher Leckie, James Bailey, Sarah Erfani"
published: "2026-07-16"
created: 2026-07-20
description: "Vision-language pre-trained models (VLPs) are widely used in real-world applications. However, they remain vulnerable to adversarial attacks. Although adversarial detection methods have demonstrated success in single-modality settings (either vision or language), their effectiveness and reliability in multimodal models such as VLPs remain largely unexplored. In this work, we study the geometry of VLP embedding space…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/nlp
  - keyword/multimodal
  - keyword/retrieval
  - keyword/evaluation
  - keyword/safety
---

# GeoDetect: Geometric Adversarial Detection for VLPs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.14737v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.14737v1
- pdf:: https://arxiv.org/pdf/2607.14737v1
- categories:: cs.CV, cs.LG

## Abstract / Summary
Vision-language pre-trained models (VLPs) are widely used in real-world applications. However, they remain vulnerable to adversarial attacks. Although adversarial detection methods have demonstrated success in single-modality settings (either vision or language), their effectiveness and reliability in multimodal models such as VLPs remain largely unexplored. In this work, we study the geometry of VLP embedding spaces and observe structured anisotropy that differs from unimodal vision models. Our theoretical analysis shows that under this anisotropic structure, adversarial attacks increase the expected geometric separation between clean and adversarial examples (AEs). Specifically, we demonstrate that AEs consistently exhibit greater expected distances to randomly sampled points than their clean counterparts, indicating that AEs tend to push representations out of manifold regions. Building on these insights, we propose GeoDetect, which leverages these off-manifold deviations via geometric scores to identify AEs. Through comprehensive evaluations, we show that our approach reliably detects AEs across diverse VLP architectures and threat settings, covering unimodal and multimodal attacks as well as adaptive attacks, thereby providing a robust and practical approach to improving the safety and reliability of these models.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.14737v1)
- [PDF](https://arxiv.org/pdf/2607.14737v1)
- [The Double-Ellipsoid Geometry of CLIP](https://arxiv.org/abs/2411.14517) (2024, citations: 41)
- [PIP: Detecting Adversarial Examples in Large Vision-Language Models via Attention Patterns of Irrelevant Probe Questions](https://arxiv.org/abs/2409.05076) (2024, citations: 20)
- [Goal-Guided Generative Prompt Injection Attack on Large Language Models](https://arxiv.org/abs/2404.07234) (2024, citations: 40)
- [Few-Shot Adversarial Prompt Learning on Vision-Language Models](https://arxiv.org/abs/2403.14774) (2024, citations: 47)
- [One Prompt Word is Enough to Boost Adversarial Robustness for Pre-Trained Vision-Language Models](https://arxiv.org/abs/2403.01849) (2024, citations: 67)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/nlp #keyword/multimodal #keyword/retrieval #keyword/evaluation #keyword/safety
