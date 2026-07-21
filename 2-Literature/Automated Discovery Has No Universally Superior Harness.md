---
title: "Automated Discovery Has No Universally Superior Harness"
source: "https://arxiv.org/html/2607.18235v1"
author: "Akshat Gupta, Jermaine Lei, Alexander Lu, Gopala Anumanchipalli, Leshem Choshen"
published: "2026-07-20"
created: 2026-07-22
description: "Autonomous discovery systems such as OpenEvolve and TTT-Discover are often used as general-purpose harnesses. However, in practice these are composite systems combining several design choices about archives, parent selection, exploration, and budget allocation into a single recipe. Because discovery runs are expensive and inherently stochastic, existing harnesses are often compared using too few independent trials t…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/evaluation
---

# Automated Discovery Has No Universally Superior Harness

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.18235v1)
- published:: 2026-07-20
- updated:: 2026-07-20
- arxiv_id:: 2607.18235v1
- pdf:: https://arxiv.org/pdf/2607.18235v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Autonomous discovery systems such as OpenEvolve and TTT-Discover are often used as general-purpose harnesses. However, in practice these are composite systems combining several design choices about archives, parent selection, exploration, and budget allocation into a single recipe. Because discovery runs are expensive and inherently stochastic, existing harnesses are often compared using too few independent trials to distinguish key methodological improvements from run-to-run variance. We systematically decompose OpenEvolve-style evolutionary search and the TTT-Discover search harness into its constituent components and systematically evaluate 30 budget-matched harnesses across 12 model-problem pairs using more than 3.1 million LLM rollouts and repeated-trial statistical analysis. Our results show that discovery harnesses have a generalization problem: No fixed harness is reliably superior across the evaluated model-problem pairs, and variants of OpenEvolve generally underperform simpler alternatives. Thus, harness choice is better viewed as a hyperparameter rather than as a universal recipe, and should be tailored to the specific problem and underlying model. We also find that early discovery progress predicts final performance, and use this property to present a budget-matched adaptive-allocation experiment that starts multiple harnesses, prunes weak partial runs, and reallocates compute to stronger survivors, outperforming both commitment to a randomly sampled fixed harness and a non-adaptive harness ensemble. Together, these results motivate shifting from fixed harness selection to online adaptation guided by early performance. We release all run pools including baseline null distributions for every model-problem pair as reusable statistical infrastructure against…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.18235v1)
- [PDF](https://arxiv.org/pdf/2607.18235v1)
- [Self-Harness: Harnesses That Improve Themselves](https://arxiv.org/abs/2606.09498) (2026, citations: 5)
- [HarnessForge: Joint Harness and Policy Evolution for Adaptive Agent Systems](https://arxiv.org/abs/2606.01779) (2026, citations: 3)
- [Compute Allocation in Evolutionary Search: From Depth-Breadth to Multi-Armed Bandits](https://arxiv.org/abs/2605.29268) (2026, citations: 1)
- [What Do Evolutionary Coding Agents Evolve?](https://arxiv.org/abs/2605.20086) (2026, citations: 1)
- [Code as Agent Harness](https://arxiv.org/abs/2605.18747) (2026, citations: 10)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/evaluation
