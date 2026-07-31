---
title: "Sample More, Reflect Less: Self-Refine and Reflexion Lose to Repeated Sampling at Equal Token Cost, from 1.5B to 7B"
source: "https://arxiv.org/html/2607.28576v1"
author: "Iliya Mirzaei"
published: "2026-07-30"
created: 2026-08-01
description: "Methods that make a language model plan, criticise and rewrite its own answer, reflect on mistakes, pick the best of several attempts, or debate with copies of itself nearly all make it generate far more text than a single chain of thought. Because generating more text raises accuracy by itself, a gain over one chain of thought does not show the method's idea is what helped. Wang et al. (2024) reported that a simple…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
---

# Sample More, Reflect Less: Self-Refine and Reflexion Lose to Repeated Sampling at Equal Token Cost, from 1.5B to 7B

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.28576v1)
- published:: 2026-07-30
- updated:: 2026-07-30
- arxiv_id:: 2607.28576v1
- pdf:: https://arxiv.org/pdf/2607.28576v1
- categories:: cs.CL, cs.AI, cs.LG

## Abstract / Summary
Methods that make a language model plan, criticise and rewrite its own answer, reflect on mistakes, pick the best of several attempts, or debate with copies of itself nearly all make it generate far more text than a single chain of thought. Because generating more text raises accuracy by itself, a gain over one chain of thought does not show the method's idea is what helped. Wang et al. (2024) reported that a simple baseline, sampling the same question repeatedly and keeping the most common answer, often wins once budgets are comparable, but gave point estimates with no confidence intervals or significance tests. We rerun that comparison as a designed experiment: seven methods, open models of 1.5B, 3B and 7B parameters, two mathematics benchmarks, 150 questions each. We count every generated token, including those spent on critiques, reflections, debate turns and checking, and compare each method against repeated sampling at its own measured cost. All 36 comparisons are paired by question, with bootstrap intervals and multiplicity correction. No method is reliably better than repeated sampling at equal cost anywhere. Ten are reliably worse, all of them methods where the model inspects its own output, and all 18 self-inspection comparisons are negative. The two kinds of self-inspection part company as models grow. Choosing stops hurting: taking Best-of-N's eight samples and just counting the most common answer beats letting the model pick by 8.0 and 11.3 points at 1.5B, but only 2.0 and 1.3 at 7B, no longer distinguishable from zero. Rewriting does not recover: Self-Refine and a forced Reflexion stay 3.6 to 10.1 points below baseline at 7B. Reflexion as published never triggered its own retry on the smallest model. It judged itself correct every time and silently became…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.28576v1)
- [PDF](https://arxiv.org/pdf/2607.28576v1)
- [Fair on the Surface: Transaction-Ordering Bias and MEV in Mysticeti DAG-based BFT Protocol](https://arxiv.org/abs/2607.13378) (2026, citations: 1)
- [Simplicity Paradox: Debunking myths about prompting and datasets for LLM evaluation](https://arxiv.org/abs/2607.14109) (2026, citations: 1)
- [Single-Agent LLMs Outperform Multi-Agent Systems on Multi-Hop Reasoning Under Equal Thinking Token Budgets](https://arxiv.org/abs/2604.02460) (2026, citations: 14)
- [The Sequential Edge: Inverse-Entropy Voting Beats Parallel Self-Consistency at Matched Compute](https://arxiv.org/abs/2511.02309) (2025, citations: 7)
- [Debate or Vote: Which Yields Better Decisions in Multi-Agent Large Language Models?](https://arxiv.org/abs/2508.17536) (2025, citations: 60)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark
