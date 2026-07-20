---
title: "Pretraining Data Can Be Poisoned through Computational Propaganda"
source: "https://arxiv.org/html/2607.15267v1"
author: "Victoria Graf, Hannaneh Hajishirzi, Noah A. Smith, David Kohlbrenner, Kyle Lo"
published: "2026-07-16"
created: 2026-07-20
description: "Poisoning pretraining data can introduce harmful behaviors to LMs that are difficult to detect and mitigate. Prior work on poisoning pretraining data has largely exploited established data sources such as Wikipedia, which do not represent the large scale and heterogeneity typical of pretraining corpora, and has ignored the interaction between poisoned data and data curation pipelines. We demonstrate that poisoning a…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/machine-learning
---

# Pretraining Data Can Be Poisoned through Computational Propaganda

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15267v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15267v1
- pdf:: https://arxiv.org/pdf/2607.15267v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
Poisoning pretraining data can introduce harmful behaviors to LMs that are difficult to detect and mitigate. Prior work on poisoning pretraining data has largely exploited established data sources such as Wikipedia, which do not represent the large scale and heterogeneity typical of pretraining corpora, and has ignored the interaction between poisoned data and data curation pipelines. We demonstrate that poisoning attacks on pretraining data are feasible beyond this limited setting through an existing web-scale content injection mechanism: public discussion interfaces. Additionally, to measure whether malicious content is included after web crawling and data curation, we introduce HalfLife, a novel analysis for estimating adversarial content inclusion in web-crawl based LM training data. We use HalfLife to explore the feasibility of poisoning pretraining corpora at web scale through open discussion interfaces. Our analysis demonstrates the importance of estimating whether poison injections are included in pretraining data, and establishes third-party webpage content as a possible vector for attacking language model pretraining.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15267v1)
- [PDF](https://arxiv.org/pdf/2607.15267v1)
- [Poisoning Attacks on LLMs Require a Near-constant Number of Poison Samples](https://arxiv.org/abs/2510.07192) (2025, citations: 72)
- [Winter Soldier: Backdooring Language Models at Pre-Training with Indirect Data Poisoning](https://arxiv.org/abs/2506.14913) (2025, citations: 6)
- [Organize the Web: Constructing Domains Enhances Pre-Training Data Curation](https://arxiv.org/abs/2502.10341) (2025, citations: 75)
- [The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale](https://arxiv.org/abs/2406.17557) (2024, citations: 1020)
- [DataComp-LM: In search of the next generation of training sets for language models](https://arxiv.org/abs/2406.11794) (2024, citations: 372)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/machine-learning
