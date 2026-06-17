---
title: "MolmoMotion: Language-guided 3D motion forecasting"
source: "https://huggingface.co/blog/allenai/molmomotion"
author: "Hugging Face Blog"
published: "2026-06-17"
created: 2026-06-18
description: "Machines have become remarkably good at perceiving motion. Given a video, modern models can track how objects and points move through a scene with exceptionally high confidence. But perception is inherently retrospective: it explains motion that has already happened. Many of the systems and applications we want to build need to look forward instead. A robot reaching for a cup has to anticipate how the cup will move…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/nlp
  - keyword/multimodal
---

# MolmoMotion: Language-guided 3D motion forecasting

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/allenai/molmomotion)
- published:: 2026-06-17

## Abstract / Summary
Machines have become remarkably good at perceiving motion. Given a video, modern models can track how objects and points move through a scene with exceptionally high confidence. But perception is inherently retrospective: it explains motion that has already happened. Many of the systems and applications we want to build need to look forward instead. A robot reaching for a cup has to anticipate how the cup will move before it touches it. A video generator has to know what realistic motion comes… Predicting motion is harder than observing it, but it's also far more useful in many scenarios. This idea was the motivation behind MolmoMotion , a new motion forecasting model we're releasing today. Given a video frame, 3D points marked on an object, and written instructions describing the intended action (e.g., “Move and rotate the wooden bowl with fruit on the table”), MolmoMotion predicts where those points will move over the next few seconds in 3D space—achieving substantially stronger performance than existing forecasting methods. Given an RGB observation, a set of query points on an object, and an action description, MolmoMotion predicts the object's future 3D point trajectory. These…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/nlp #keyword/multimodal
