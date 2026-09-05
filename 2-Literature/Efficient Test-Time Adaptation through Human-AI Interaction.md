---
title: "Efficient Test-Time Adaptation through Human-AI Interaction"
source: "https://arxiv.org/html/2609.04141v1"
author: "Zora Zhiruo Wang, Apurva Gandhi, Rulin Shao, Aspen Chen, Jonas Mueller, Zhiqi Liang, Jett Chen, Michael Ryan, Qianou Ma, Luxi He, Zhoujun Cheng, Andre He, Seungone Kim, Jiayi Geng, Mingqian Zheng, Weiwei Sun, Zheyuan Zhang, Xinran Zhao, Yike Wang, Abe Hou, Liwei Jiang, Pang Wei Koh, Diyi Yang, Graham Neubig, Daniel Fried"
published: "2026-09-03"
created: 2026-09-06
description: "AI agents are trained on population-scale data to encode broad capabilities spanning those of many practitioners. Yet the artifacts they produce rarely meet the personal bar professionals need to stake their reputation on. On realistic, open-ended tasks where success criteria are heterogeneous and insufficiently documented, individual expertise lives precisely in the elevation and departure from the average. In prac…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/agents
  - keyword/machine-learning
---

# Efficient Test-Time Adaptation through Human-AI Interaction

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.04141v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.04141v1
- pdf:: https://arxiv.org/pdf/2609.04141v1
- categories:: cs.AI

## Abstract / Summary
AI agents are trained on population-scale data to encode broad capabilities spanning those of many practitioners. Yet the artifacts they produce rarely meet the personal bar professionals need to stake their reputation on. On realistic, open-ended tasks where success criteria are heterogeneous and insufficiently documented, individual expertise lives precisely in the elevation and departure from the average. In practice, iterative human-agent interaction surfaces criteria that users cannot fully specify up front, yet apply repeatedly across tasks. We argue this cross-session interaction data is a rich, underused signal for closing the gap to individual expertise. In this work, we propose test-time adaptation through human-agent interaction (TAHI), which integrates these signals into agent context and weights, and crystallizes each user's training and evaluation criteria via an evolving rubric module. We adapt agents to 30 individuals in two high-utility domains, writing and visual creation, on a total of 600 tasks. Our agents improve solo task success by 4.5-20.9% within only tens of tasks. Meanwhile, our evolving rubric module serves as a scalable annotation tool, creating evaluation rubrics that catch 16.0-22.3% more failures than those from LMs or humans alone. While agents are adapted towards individuals, we show these personalized agents also produce improvements in success of up to 8.8% that generalize across users.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.04141v1)
- [PDF](https://arxiv.org/pdf/2609.04141v1)
- [What do you mean by human-AI collaboration: Prerequisite functions and the affordances needed to achieve it](https://arxiv.org/abs/2606.15509) (2026, citations: 1)
- [Learning, Fast and Slow: Towards LLMs That Adapt Continually](https://arxiv.org/abs/2605.12484) (2026, citations: 3)
- [CollabSkill: Evaluating Human-Agent Collaboration On Real-World Tasks](https://arxiv.org/abs/2606.09833) (2026, citations: 1)
- [Gym-Anything: Turn any Software into an Agent Environment](https://arxiv.org/abs/2604.06126) (2026, citations: 16)
- [How LLMs Distort Our Written Language](https://arxiv.org/abs/2603.18161) (2026, citations: 20)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/agents #keyword/machine-learning
