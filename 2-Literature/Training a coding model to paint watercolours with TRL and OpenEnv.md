---
title: "Training a coding model to paint watercolours with TRL and OpenEnv"
source: "https://huggingface.co/blog/train-to-paint-with-code"
author: "Hugging Face Blog"
published: "2026-09-03"
created: 2026-09-04
description: "On 23 August, Surya Narreddi posted a beautiful video of watercolours painted by a language model. The model writes JavaScript through p5.brush , a library that 'adds natural drawing tools to p5.js'. The video went viral fast, over 1.5M views at the time of writing. The video came with a blog post explaining the training behind an earlier and narrower stage of the project, close-up flowers rather than the full compo…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/agents
  - keyword/machine-learning
---

# Training a coding model to paint watercolours with TRL and OpenEnv

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/train-to-paint-with-code)
- published:: 2026-09-03

## Abstract / Summary
On 23 August, Surya Narreddi posted a beautiful video of watercolours painted by a language model. The model writes JavaScript through p5.brush , a library that "adds natural drawing tools to p5.js". The video went viral fast, over 1.5M views at the time of writing. The video came with a blog post explaining the training behind an earlier and narrower stage of the project, close-up flowers rather than the full compositions in the video, sadly without open artifacts yet. His site says a full technical report is coming, so ensure you follow him. The original idea is his, coming from the art and design side, where his skills are way beyond mine . My attempt is on the engineering side, reproducing the recipe in the open with every piece published. Note: for the context behind the project, told by Surya himself, watch this video of his thesis . In this article I try and reproduce his idea with TRL and OpenEnv . The reference pool dataset, the RL environment, the training scripts and the trained models, all open. Once the two Spaces are up, the recipe is one command. Duplicate the environment and the scorer model , set two environment variables for the reward mix, and launch: hf jobs uv…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/agents #keyword/machine-learning
