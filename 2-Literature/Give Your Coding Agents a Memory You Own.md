---
title: "Give Your Coding Agents a Memory You Own"
source: "https://huggingface.co/blog/funes"
author: "Hugging Face Blog"
published: "2026-09-03"
created: 2026-09-04
description: "Earlier this year, Software Forgets: Agent Traces Are the Memory made the case that coding agents already produce the record we keep losing. As they search a codebase, try approaches, hit errors, read documentation, and change direction, they leave behind a dense account of not just what changed, but why . While the diagnosis is correct, traces are only potential memory. The session logs of an agent are still just a…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/retrieval
  - keyword/evaluation
  - keyword/agents
  - keyword/machine-learning
---

# Give Your Coding Agents a Memory You Own

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/funes)
- published:: 2026-09-03

## Abstract / Summary
Earlier this year, Software Forgets: Agent Traces Are the Memory made the case that coding agents already produce the record we keep losing. As they search a codebase, try approaches, hit errors, read documentation, and change direction, they leave behind a dense account of not just what changed, but why . While the diagnosis is correct, traces are only potential memory. The session logs of an agent are still just an archive. You cannot grep your way to “why did we move off the streaming parser?” across ten thousand turns. For an agent to use those traces while it works, they need indexing, retrieval, ranking, and exact provenance. That is what funes provides. It is a durable memory layer for your agents (Claude Code, Codex, pi, and Hermes). It is built from the sessions already on your machine. It works locally and becomes part of your agent's normal workflow with one command. When you want it to, it can also travel to a Hugging Face dataset you own, private by default. Add memory to the agent you already use funes is a single binary. Its default inference backend has no ML runtime dependency, and embedding and reranking happen on your machine . Install it: curl -fsSL https://hug…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/retrieval #keyword/evaluation #keyword/agents #keyword/machine-learning
