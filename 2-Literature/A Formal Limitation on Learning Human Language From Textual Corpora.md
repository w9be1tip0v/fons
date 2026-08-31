---
title: "A Formal Limitation on Learning Human Language From Textual Corpora"
source: "https://arxiv.org/html/2608.28560v1"
author: "Emily Cheng, Ryan Cotterell"
published: "2026-08-28"
created: 2026-09-01
description: "Can a listener recover what a speaker means from the form of an utterance alone? We answer this question information-theoretically, and for a listener given by any featurizer of text, including the hidden states of contemporary large language models. Modeling language use as a joint distribution over meanings, contexts, and utterances, we derive upper bounds on the probability that a decoder recovers a speaker's int…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
---

# A Formal Limitation on Learning Human Language From Textual Corpora

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.28560v1)
- published:: 2026-08-28
- updated:: 2026-08-28
- arxiv_id:: 2608.28560v1
- pdf:: https://arxiv.org/pdf/2608.28560v1
- categories:: cs.CL

## Abstract / Summary
Can a listener recover what a speaker means from the form of an utterance alone? We answer this question information-theoretically, and for a listener given by any featurizer of text, including the hidden states of contemporary large language models. Modeling language use as a joint distribution over meanings, contexts, and utterances, we derive upper bounds on the probability that a decoder recovers a speaker's intended meaning from a representation of the utterance. The bounds are governed by the uncertainty that form leaves about meaning, which splits into an irreducible part and a part that only (extralinguistic) context, but never the utterance alone, can resolve. Because these quantities are intrinsic to language, no representation, however much text or supervision produced it, can surpass them; the bounds hold whether the space of meanings is discrete or continuous. Experiments on artificial languages, Mandarin zero-pronoun resolution, and color reference provide empirical evidence in support of the theory.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.28560v1)
- [PDF](https://arxiv.org/pdf/2608.28560v1)
- [Language Models are Injective and Hence Invertible](https://arxiv.org/abs/2510.15511) (2025, citations: 35)
- [Pragmatics in the Era of Large Language Models: A Survey on Datasets, Evaluation, Opportunities and Challenges](https://arxiv.org/abs/2502.12378) (2025, citations: 46)
- [LLMs as a synthesis between symbolic and distributed approaches to language](https://arxiv.org/abs/2502.11856) (2025, citations: 6)
- [How linguistics learned to stop worrying and love the language models](https://arxiv.org/abs/2601.10421) (2025, citations: 66)
- [Why do objects have many names? A study on word informativeness in language use and lexical systems](https://arxiv.org/abs/2410.07827) (2024, citations: 4)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp
