---
title: "SWE-Prime: Fewer Trajectories, Better Performance"
source: "https://arxiv.org/html/2608.27449v1"
author: "Dewu Zheng, Ruizhe Ye, Yanlin Wang, Yang Ye, Hongyu Zhang, Ensheng Shi, Xilin Liu, Yuchi Ma, Jianxing Yu, Zibin Zheng"
published: "2026-08-27"
created: 2026-08-29
description: "To improve large language models' ability to resolve real-world software issues, prior work has focused on constructing large-scale agent trajectory datasets and performing supervised fine-tuning (SFT) on successful trajectories. However, task success does not guarantee high-quality supervision: successful trajectories may still contain ineffective, redundant, or risky steps. Directly using such trajectories for SFT…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/agents
  - keyword/machine-learning
---

# SWE-Prime: Fewer Trajectories, Better Performance

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27449v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27449v1
- pdf:: https://arxiv.org/pdf/2608.27449v1
- categories:: cs.SE, cs.AI, cs.CL

## Abstract / Summary
To improve large language models' ability to resolve real-world software issues, prior work has focused on constructing large-scale agent trajectory datasets and performing supervised fine-tuning (SFT) on successful trajectories. However, task success does not guarantee high-quality supervision: successful trajectories may still contain ineffective, redundant, or risky steps. Directly using such trajectories for SFT can introduce noisy supervision and encourage models to imitate undesirable problem-solving behaviors. Therefore, we propose SWE-Prime, a multi-granularity, two-stage SFT data selection method that progressively filters training data at the trajectory and segment levels. Specifically, the first stage performs trajectory-level screening based on process quality, result quality, and data representativeness, selecting a high-quality and representative subset of successful trajectories. The second stage performs segment-level selection by grouping consecutive steps into semantic segments and assessing each segment based on its contribution to the final solution, learnability, and potential risks. During SFT, all segments remain in the sequence to preserve context, while only selected segments contribute to the loss computation. Experiments on SWE-Bench Pro and SWE-Bench Verified show that training on the 10% trajectory subset selected by SWE-Prime outperforms training on the full resolved dataset, yielding relative performance gains of up to 12.2% and 24.2%, respectively.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27449v1)
- [PDF](https://arxiv.org/pdf/2608.27449v1)
- [PhoenixRepair: Rethinking Repair Strategy Exploration in Software Agents](https://arxiv.org/abs/2607.18859) (2026, citations: 1)
- [SWE-Next: Scalable Real-World Software Engineering Tasks for Agents](https://arxiv.org/abs/2603.20691) (2026, citations: 7)
- [SWE-Master: Unleashing the Potential of Software Engineering Agents via Post-Training](https://arxiv.org/abs/2602.03411) (2026, citations: 12)
- [SERA: Soft-Verified Efficient Repository Agents](https://arxiv.org/abs/2601.20789) (2026, citations: 10)
- [Advances and Frontiers of LLM-based Issue Resolution in Software Engineering: A Comprehensive Survey](https://arxiv.org/abs/2601.11655) (2026, citations: 8)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/agents #keyword/machine-learning
