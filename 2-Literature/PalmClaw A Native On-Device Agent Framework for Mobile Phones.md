---
title: "PalmClaw: A Native On-Device Agent Framework for Mobile Phones"
source: "https://arxiv.org/html/2607.13027v1"
author: "Hongru Cai, Yongqi Li, Ran Wei, Wenjie Li"
published: "2026-07-14"
created: 2026-07-16
description: "Open-source on-device mobile agent framework that manages sessions, memory, skills, tools, and the agent loop natively, exposing device capabilities as explicit tools with clear execution boundaries and large speedups over GUI baselines."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/ai
  - keyword/agents
  - keyword/machine-learning
  - keyword/research-paper
---

# PalmClaw: A Native On-Device Agent Framework for Mobile Phones

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.13027v1)
- published:: 2026-07-14
- updated:: 2026-07-14
- arxiv_id:: 2607.13027v1
- pdf:: https://arxiv.org/pdf/2607.13027v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
Large Language Model (LLM) agents have moved beyond generating responses to executing multi-step tasks by calling tools, observing the results, and iteratively deciding the next action. Most agent systems run on desktops or servers, which support tool use and task automation. Mobile devices are also important agent environments because they are widely accessible and contain users' data, sensors, and daily-use applications. Existing mobile agents mainly operate smartphones through graphical user interface (GUI) actions such as tapping, swiping, and typing, which often form long, interface-dependent sequences, cannot directly access device capabilities, and make execution boundaries difficult to define. We present PalmClaw, an open-source agent framework that runs natively on mobile phones and manages the sessions, memory, skills, tools, and agent loop directly on the device. PalmClaw exposes device capabilities as device tools with explicit arguments, structured results, and clearly defined execution boundaries. This design enables agents to use mobile capabilities directly while keeping each action explicit and controlled. Experiments show an 11.5% relative improvement in task success and a 94.9% reduction in completion time over the strongest baseline, with lower setup burden and traces illustrating how execution boundaries are applied. Code is available at https://github.com/ModalityDance/PalmClaw.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.13027)
- [PDF](https://arxiv.org/pdf/2607.13027v1)
- [Code](https://github.com/ModalityDance/PalmClaw)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/ai #keyword/agents #keyword/machine-learning #keyword/research-paper
