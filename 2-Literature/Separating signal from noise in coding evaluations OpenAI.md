---
title: "Separating signal from noise in coding evaluations | OpenAI"
source: "https://openai.com/index/separating-signal-from-noise-coding-evaluations"
author: "OpenAI"
published: "2026-07-08"
created: 2026-07-13
description: "OpenAI audits SWE-Bench Pro and estimates roughly 30% of tasks are broken due to overly strict tests, underspecified prompts, low-coverage tests, and misleading prompts, retracting its earlier recommendation to adopt the benchmark."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/openai
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
  - keyword/safety
---

# Separating signal from noise in coding evaluations | OpenAI

## Source Metadata
- type:: blog
- source:: [OpenAI News](https://openai.com/index/separating-signal-from-noise-coding-evaluations)
- published:: 2026-07-08

## Abstract / Summary
OpenAI argues that flawed coding benchmarks can distort deployment and safety decisions. After previously discouraging SWE-bench Verified and pointing the community to SWE-Bench Pro, the team audited the 731-task public split of SWE-Bench Pro with an automated datapoint analysis pipeline plus human-supervised agent review and a five-engineer annotation campaign. They report evidence of breaking issues in a large fraction of the dataset: the agent pipeline flagged about 27.4% of tasks as broken, while human annotation identified about 34.1%. Dominant failure modes include overly strict tests that enforce unspecified implementation details, underspecified prompts, low-coverage tests that let incomplete fixes pass, and misleading prompts that conflict with hidden tests. OpenAI estimates ~30% of SWE-Bench Pro tasks are broken and retracts its earlier recommendation to adopt the benchmark, calling for harder-to-game evaluations built with stronger human oversight.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [OpenAI News](https://openai.com/news/)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/openai #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/safety
