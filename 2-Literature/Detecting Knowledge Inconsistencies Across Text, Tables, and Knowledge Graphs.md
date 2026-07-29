---
title: "Detecting Knowledge Inconsistencies Across Text, Tables, and Knowledge Graphs"
source: "https://arxiv.org/html/2607.25959v1"
author: "Fanfu Wei, Thibault Ehrhart, Raphaël Troncy"
published: "2026-07-28"
created: 2026-07-30
description: "Wikipedia and Wikidata are widely used for information access, LLM pre-training, and retrieval-augmented generation. Their knowledge is deeply connected but scattered across text, tables, and knowledge graphs. This raises a practical question: when these modalities disagree, how can we detect and explain the conflict? We study this problem as \emph{modality-level inconsistency detection}. We first introduce a taxono…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/machine-learning
---

# Detecting Knowledge Inconsistencies Across Text, Tables, and Knowledge Graphs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.25959v1)
- published:: 2026-07-28
- updated:: 2026-07-28
- arxiv_id:: 2607.25959v1
- pdf:: https://arxiv.org/pdf/2607.25959v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Wikipedia and Wikidata are widely used for information access, LLM pre-training, and retrieval-augmented generation. Their knowledge is deeply connected but scattered across text, tables, and knowledge graphs. This raises a practical question: when these modalities disagree, how can we detect and explain the conflict? We study this problem as \emph{modality-level inconsistency detection}. We first introduce a taxonomy of cross-modal knowledge inconsistencies, covering information granularity differences, direct conflicts, temporal changes, and KG incompleteness. We then present \textsc{Kontrast}, an automatic framework that uses Text-to-SPARQL and LLM reasoning to compare table-based answers with KG evidence and categorize the resulting inconsistencies. Experiments on various Table-QA datasets show that cross-modal inconsistencies are common and informative. They reveal not only true knowledge conflicts, but also missing KG structure and temporal mismatches while being limited by Text-to-SPARQL errors and noise. Our analysis shows that text, tables, and KGs can complement and correct one another through systematic comparison. \textsc{Kontrast} provides a practical tool for large-scale knowledge auditing and establishes a benchmark for future work on cross-modal knowledge consistency. Code and data are available at https://github.com/ECLADATTA/KONTRAST.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.25959v1)
- [PDF](https://arxiv.org/pdf/2607.25959v1)
- [WikiConflict: A New Dataset for Conflicting Data Reconciliation in Knowledge Graph Construction](https://doi.org/10.1145/3731443.3771371) (2025, citations: 1)
- [Detecting Corpus-Level Knowledge Inconsistencies in Wikipedia with Large Language Models](https://arxiv.org/abs/2509.23233) (2025, citations: 4)
- [Consensus or Conflict? Fine-Grained Evaluation of Conflicting Answers in Question-Answering](https://arxiv.org/abs/2508.12355) (2025, citations: 4)
- [MoNaCo: More Natural and Complex Questions for Reasoning Across Dozens of Documents](https://arxiv.org/abs/2508.11133) (2025, citations: 23)
- [GRASP: Generic Reasoning And SPARQL Generation across Knowledge Graphs - Demo System](https://arxiv.org/abs/2507.08107) (2025, citations: 9)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/machine-learning
