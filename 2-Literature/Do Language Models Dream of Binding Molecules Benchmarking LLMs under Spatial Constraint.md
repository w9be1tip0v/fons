---
title: "Do Language Models Dream of Binding Molecules? Benchmarking LLMs under Spatial Constraints"
source: "https://arxiv.org/html/2607.18144v1"
author: "Thomas MacDougall, Maksim Kuznetsov, Roman Schutski, Rim Shayakhmetov, Maxim Malkov, Vladimir Aladinskiy, Alex Aliper, Alex Zhavoronkov"
published: "2026-07-20"
created: 2026-07-22
description: "Structure-based drug design (SBDD) leverages the 3D structure of protein targets, often complemented by other spatial constraints, to generate candidate binding molecules. While diffusion models have dominated as a leading paradigm for high-quality 3D molecule generation, LLM-based methods are rapidly emerging in molecular design and have shown competitive performance in pocket-conditioned molecular generation. Howe…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/diffusion
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
---

# Do Language Models Dream of Binding Molecules? Benchmarking LLMs under Spatial Constraints

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.18144v1)
- published:: 2026-07-20
- updated:: 2026-07-20
- arxiv_id:: 2607.18144v1
- pdf:: https://arxiv.org/pdf/2607.18144v1
- categories:: cs.LG, cs.AI, cs.CL

## Abstract / Summary
Structure-based drug design (SBDD) leverages the 3D structure of protein targets, often complemented by other spatial constraints, to generate candidate binding molecules. While diffusion models have dominated as a leading paradigm for high-quality 3D molecule generation, LLM-based methods are rapidly emerging in molecular design and have shown competitive performance in pocket-conditioned molecular generation. However, their ability to reason about physics and 3D spatial environments is largely underexplored. In this work, we systematically analyze whether current general-purpose LLMs are capable of navigating complex 3D constraints compared to established baselines such as specialized diffusion models. We consider 3D ligand generation conditioned on protein pockets together with ligand- and interaction-derived spatial constraints, including anchor fragments, pharmacophore points, and mandatory pocket-ligand interactions. To enable this evaluation, we introduce 3D-Fit - a token-efficient benchmarking strategy for assessing LLM performance on multi-conditioned spatial molecule generation. Our findings reveal a clear pattern in LLM spatial capabilities: while they still lag behind state-of-the-art approaches, they are promising and can handle multiple spatial constraints simultaneously, enabling scaling to heterogeneous setups.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.18144v1)
- [PDF](https://arxiv.org/pdf/2607.18144v1)
- [Steering semi-flexible molecular diffusion model for structure-based drug design with reinforcement learning](https://www.semanticscholar.org/paper/abe13026c4f1e39219db54215121cd8f1ef0948d) (2026, citations: 2)
- [Interaction-constrained 3D molecular generation using a diffusion model enables structure-based pharmacophore modeling for drug design](https://www.nature.com/articles/s44386-026-00040-x.pdf) (2026, citations: 2)
- [Unified modeling of 3D molecular generation via atomic interactions with PocketXMol.](https://doi.org/10.1016/j.cell.2026.01.003) (2026, citations: 10)
- [An effective fragment-based dual conditional diffusion framework for molecular generation](https://www.semanticscholar.org/paper/32ce64eb07553d91973be8d9694029764d9e346f) (2026, citations: 1)
- [SGEDiff: a subgraph-enriched diffusion model for structure-based 3D molecular generation](https://link.springer.com/content/pdf/10.1186/s13321-025-01123-z.pdf) (2025, citations: 1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/diffusion #keyword/retrieval #keyword/evaluation #keyword/benchmark
