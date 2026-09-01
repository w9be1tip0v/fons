---
title: "The First Token Is a Clue: Verbalizing Multi-Token Concepts from the J-lens"
source: "https://arxiv.org/html/2608.31084v1"
author: "Xijie Gong, Tonghan Wang"
published: "2026-08-31"
created: 2026-09-02
description: "The Jacobian Lens (J-lens) is a recent tool for interpreting LLMs. It reads a hidden state as a ranked list of vocabulary tokens, leaving multi-token concepts without a representation of their own. The original J-lens work addresses this limitation with Template Lens, which precomputes vectors for a fixed phrase vocabulary, and Oracle Lens, which fine-tunes components to propose phrases and reconstruct phrase vector…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/retrieval
---

# The First Token Is a Clue: Verbalizing Multi-Token Concepts from the J-lens

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.31084v1)
- published:: 2026-08-31
- updated:: 2026-08-31
- arxiv_id:: 2608.31084v1
- pdf:: https://arxiv.org/pdf/2608.31084v1
- categories:: cs.CL

## Abstract / Summary
The Jacobian Lens (J-lens) is a recent tool for interpreting LLMs. It reads a hidden state as a ranked list of vocabulary tokens, leaving multi-token concepts without a representation of their own. The original J-lens work addresses this limitation with Template Lens, which precomputes vectors for a fixed phrase vocabulary, and Oracle Lens, which fine-tunes components to propose phrases and reconstruct phrase vectors. We ask whether multi-token concepts and their vectors can instead be recovered directly from J-lens and the frozen model. We find that the first token of a multi-token concept is about as readable as a single-token concept. Given the correct first token and source prompt, the frozen model recovers the second token in 88.3% of two-token cases. We show that a vector for the complete concept can be recovered from subsequent hidden states in a single forward pass. We therefore use J-lens to propose first tokens and let the frozen model complete candidate concepts. We then recover a vector for each candidate and score it alongside the complete vocabulary. Across 496 multi-hop clozes on Gemma-3-12B-IT, Llama-3.1-8B, and Qwen3-14B, our method achieves an average $\mathrm{Rank@}10$ of 43.1%, compared with 27.6% for Template Lens. Without the J-lens clue, performance drops to 21.6%, showing that the first-token clue substantially improves readout. Causal concept swaps using the recovered vectors achieve an average $\mathrm{succ}@10$ of 61.4%, compared with 26.2% for Template Lens under the same intervention. These results show that first-token clues can guide multi-token concept recovery, while subsequent hidden states provide vectors for readout and intervention.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.31084v1)
- [PDF](https://arxiv.org/pdf/2608.31084v1)
- [Verbalizable Representations Form a Global Workspace in Language Models](https://arxiv.org/abs/2607.15495) (2026, citations: 35)
- [From Tokens to Words: On the Inner Lexicon of LLMs](https://arxiv.org/abs/2410.05864) (2024, citations: 50)
- [Token Erasure as a Footprint of Implicit Vocabulary Items in LLMs](https://arxiv.org/abs/2406.20086) (2024, citations: 24)
- [Hopping Too Late: Exploring the Limitations of Large Language Models on Multi-Hop Queries](https://arxiv.org/abs/2406.12775) (2024, citations: 103)
- [SelfIE: Self-Interpretation of Large Language Model Embeddings](https://arxiv.org/abs/2403.10949) (2024, citations: 70)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/retrieval
