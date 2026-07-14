---
title: "Verifying Rust cryptography in SymCrypt, from standards to code"
source: "https://www.microsoft.com/en-us/research/blog/verifying-rust-cryptography-in-symcrypt-from-standards-to-code/"
author: "Microsoft Research Blog"
published: "2026-07-13"
created: 2026-07-15
description: "Microsoft open-sources verified Rust ML-KEM and SHA-3 in SymCrypt using Aeneas/Lean; AI agents help write independently checkable proofs."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/microsoft
  - keyword/agents
  - keyword/ai
  - keyword/safety
  - keyword/machine-learning
---

# Verifying Rust cryptography in SymCrypt, from standards to code

## Source Metadata
- type:: blog
- source:: [Microsoft Research Blog](https://www.microsoft.com/en-us/research/blog/verifying-rust-cryptography-in-symcrypt-from-standards-to-code/)
- published:: 2026-07-13

## Abstract / Summary
Microsoft describes verifying production cryptographic algorithms written in Rust for SymCrypt using the Aeneas toolchain and Lean proofs. Initial public branch includes complete proofs for ML-KEM and SHA-3 used in Windows Insider builds. Agents write proofs and intermediate properties while compilation, extraction, and proof checking remain deterministic. Methodology targets post-quantum and other performance-critical crypto with human review of standard formalizations.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Microsoft Research Blog](https://www.microsoft.com/en-us/research/blog/)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/microsoft #keyword/agents #keyword/ai #keyword/safety #keyword/machine-learning
