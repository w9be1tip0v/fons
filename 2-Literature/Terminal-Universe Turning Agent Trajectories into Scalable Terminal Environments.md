---
title: "Terminal-Universe: Turning Agent Trajectories into Scalable Terminal Environments"
source: "https://arxiv.org/html/2609.04148v1"
author: "Jie Wu, Zhenru Zhang, Beichen Zhang, Xuwu Wang, Yuhui Su, Mouxiang Chen, Peng Wang, Zhihai Wang, Que Shen, Hao Zhou, An Yang, Fei Huang, Yujiu Yang, Dayiheng Liu"
published: "2026-09-03"
created: 2026-09-06
description: "As terminal-based code agents become prevalent, agent trajectories have accumulated at scale, while realistic, executable environments remain scarce. However, environments are what agent post-training actually requires: each can be re-queried into many verifiable tasks and provides execution feedback, whereas a trajectory is a single frozen demonstration. Rather than generating environments from scratch, we observe…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/evaluation
  - keyword/agents
  - keyword/machine-learning
---

# Terminal-Universe: Turning Agent Trajectories into Scalable Terminal Environments

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.04148v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.04148v1
- pdf:: https://arxiv.org/pdf/2609.04148v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
As terminal-based code agents become prevalent, agent trajectories have accumulated at scale, while realistic, executable environments remain scarce. However, environments are what agent post-training actually requires: each can be re-queried into many verifiable tasks and provides execution feedback, whereas a trajectory is a single frozen demonstration. Rather than generating environments from scratch, we observe that the tool-execution history in existing trajectories exposes the structure and contents of the environments in which they ran, making it possible to reconstruct those environments from the trajectories themselves. Thus, we introduce Terminal-Universe, a framework which turns each trajectory into a reusable environment and explores it for synthesizing new tasks and continued interactions. Specifically, Terminal-Universe replays the file operations recorded in a trajectory to restore each file before the agent modified it, yielding a partial workspace; a completion agent then supplies the missing files and dependencies. On this recovered workspace, we both reconstruct the original intent task and synthesize entirely new ones. Besides, we also scale the tasks along two complementary axes: breadth and depth. For breadth, we mine directional dependency relations between related environments and synthesize cross-workspace queries spanning multiple codebases, as developers routinely do in real-world development. For depth, we extend the initial single-turn query into a multi-round session that captures iterative user feedback and requirement refinement via a user agent. Applied to public terminal agent trajectories, Terminal-Universe produces 37.3k task-sufficient environments. Supervised fine-tuning of Qwen3.5-27B on this corpus improves single-round performan…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.04148v1)
- [PDF](https://arxiv.org/pdf/2609.04148v1)
- [FACET: Preserving Source Intent and Executable State in Terminal Task Synthesis](https://arxiv.org/abs/2608.18580) (2026, citations: 1)
- [CalibForge: Adversarial Solver Calibration for Scaling Learnable Terminal Tasks](https://arxiv.org/abs/2608.06352) (2026, citations: 1)
- [Recursive Synthesis for Long-Horizon Terminal Tasks](https://arxiv.org/abs/2608.05466) (2026, citations: 3)
- [Meta-Task: Turning Terminal Task Synthesis into a Terminal Task for Scalable Agent Training](https://arxiv.org/abs/2607.27929) (2026, citations: 1)
- [ICAE-Bench: Evaluating Coding Agents as Interactive Project Builders](https://arxiv.org/abs/2607.21217) (2026, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/evaluation #keyword/agents #keyword/machine-learning
