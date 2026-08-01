---
title: "Rethinking Inference-Time Scaling in Local Computer-Use Agents: Failure Modes and Compute Tradeoffs"
source: "https://arxiv.org/html/2607.28573v1"
author: "Woongkyu Lee, Jungwook Choi"
published: "2026-07-30"
created: 2026-08-02
description: "Deploying autonomous computer-use agents (CUAs) locally is increasingly important for privacy, cost efficiency, and practical usability, yet improving their performance under strict hardware constraints remains challenging. While recent studies show that inference-time scaling can improve frontier computer-use agents through additional computation during execution, its effectiveness for resource-constrained local mo…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
  - keyword/machine-learning
---

# Rethinking Inference-Time Scaling in Local Computer-Use Agents: Failure Modes and Compute Tradeoffs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.28573v1)
- published:: 2026-07-30
- updated:: 2026-07-30
- arxiv_id:: 2607.28573v1
- pdf:: https://arxiv.org/pdf/2607.28573v1
- categories:: cs.AI

## Abstract / Summary
Deploying autonomous computer-use agents (CUAs) locally is increasingly important for privacy, cost efficiency, and practical usability, yet improving their performance under strict hardware constraints remains challenging. While recent studies show that inference-time scaling can improve frontier computer-use agents through additional computation during execution, its effectiveness for resource-constrained local models remains poorly understood. We present a systematic empirical study of inference-time scaling in local CUAs across contextual, temporal, structural, and parallel dimensions. We evaluate Qwen3-VL-8B/30B-A3B, UI-TARS-1.5-7B, and OpenCUA-7B on the OSWorld benchmark. Our results show that additional computation often yields diminishing returns while changing failure modes. Contextual scaling provides historical grounding that improves trajectory stability and task accuracy, but its gains saturate as token cost increases and failures shift from repetitive or stalled trajectories toward premature false successes. Temporal scaling similarly reduces max-step stalls, yet does not substantially improve task success, indicating that longer horizons often extend erroneous trajectories rather than correct them. We further find that structural decomposition can introduce planning and formatting overhead in local two-stage agents, while parallel scaling partially mitigates these failures at a substantial computational cost. Overall, our findings suggest that efficient local CUAs require selective compute allocation, failure-aware control mechanisms, and agentic frameworks designed around the capabilities and limitations of local models.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.28573v1)
- [PDF](https://arxiv.org/pdf/2607.28573v1)
- [Step-level Optimization for Efficient Computer-use Agents](https://arxiv.org/abs/2604.27151) (2026, citations: 1)
- [PAL-UI: Planning with Active Look-back for Vision-Based GUI Agents](https://arxiv.org/abs/2510.00413) (2025, citations: 8)
- [GUI-KV: Efficient GUI Agents via KV Cache with Spatio-Temporal Awareness](https://arxiv.org/abs/2510.00536) (2025, citations: 7)
- [CoAct-1: Computer-using Multi-Agent System with Coding Actions](https://arxiv.org/abs/2508.03923) (2025, citations: 23)
- [GTA1: GUI Test-time Scaling Agent](https://arxiv.org/abs/2507.05791) (2025, citations: 90)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/machine-learning
