---
title: "Grabette: an open system to record robot-manipulation data"
source: "https://huggingface.co/blog/grabette"
author: "Hugging Face Blog"
published: "2026-07-21"
created: 2026-07-22
description: "The bottleneck isn’t the model. It’s the data. Robot learning has a supply problem. We have capable policy architectures (transformer-based VLAs, diffusion and flow-matching policies, and even world models) and the GPUs to train them. What we lack is large, diverse, real-world manipulation data. Teleoperating a robot to collect it can be expensive and demanding: first of all, it requires a robot . And depending on t…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/transformer
  - keyword/multimodal
  - keyword/diffusion
---

# Grabette: an open system to record robot-manipulation data

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/grabette)
- published:: 2026-07-21

## Abstract / Summary
The bottleneck isn’t the model. It’s the data. Robot learning has a supply problem. We have capable policy architectures (transformer-based VLAs, diffusion and flow-matching policies, and even world models) and the GPUs to train them. What we lack is large, diverse, real-world manipulation data. Teleoperating a robot to collect it can be expensive and demanding: first of all, it requires a robot . And depending on the teleoperation method, data collection can be tedious for the user if it takes hours and involve significant hardware and logistical challenges. That is difficult to scale with the wide variety of tasks and environnements required. But you don't need a robot to collect robot data. Just a human hand, a gripper, a camera, and a way to recover the 6-DoF trajectory of what the hand did. Capture the demonstration and you have data a robot can learn from. That's what we're releasing today: Grabette, an open, low-cost system for recording manipulation data. Pick it up, record a task with your own hand, and get back a clean, robot-ready dataset. No robot, no lab, no teleop rig. And that's the bigger goal: if recording a demonstration is as easy as shooting a video, anyone can…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/transformer #keyword/multimodal #keyword/diffusion
