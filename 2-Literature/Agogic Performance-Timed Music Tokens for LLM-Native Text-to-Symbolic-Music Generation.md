---
title: "Agogic: Performance-Timed Music Tokens for LLM-Native Text-to-Symbolic-Music Generation"
source: "https://arxiv.org/html/2608.03999v1"
author: "Junhao Chen, Mingjin Chen, Jingjia Mao, Lin Chen, Saining Zhang, Minglin Chen, Ruocheng Wu, Liaoyuan Fan, Wenyi Li, Mingju Gao, Henghaofan Zhang, Zhihao Li, Hao Zhao, Yufei Wang, Ruqi Huang"
published: "2026-08-04"
created: 2026-08-06
description: "Text-to-music language models begin with a choice usually made by default: how to tokenize music. Normally entangled with backbone, data, and recipe, its effect has never been measured in isolation. We fix pretrained Qwen3.5 (0.8B-27B), data, budget, and decoding, and swap only the representation across seven tokenizations, anchoring texture metrics to each representation's model-free ceiling. The ordering is clean…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/machine-learning
---

# Agogic: Performance-Timed Music Tokens for LLM-Native Text-to-Symbolic-Music Generation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.03999v1)
- published:: 2026-08-04
- updated:: 2026-08-04
- arxiv_id:: 2608.03999v1
- pdf:: https://arxiv.org/pdf/2608.03999v1
- categories:: cs.SD, cs.CL

## Abstract / Summary
Text-to-music language models begin with a choice usually made by default: how to tokenize music. Normally entangled with backbone, data, and recipe, its effect has never been measured in isolation. We fix pretrained Qwen3.5 (0.8B-27B), data, budget, and decoding, and swap only the representation across seven tokenizations, anchoring texture metrics to each representation's model-free ceiling. The ordering is clean and surprising: representation, not model size, is the binding variable for distributional fidelity. Scaling the backbone 34x barely moves Frechet Music Distance (FMD), whereas switching representation halves it. PMT, a performance-resolution stream we release (10 ms timing, per-note velocity, multi-track texture; 609 symbols), reaches FMD 159 at 0.8B against 272-286 for beat grids (1.7-1.8x lower, up to 2.8x elsewhere; non-overlapping bootstrap CIs), so a 0.8B performance-resolution model beats a 27B beat grid. It reappears on a 26M from-scratch backbone and a second performance-resolution tokenizer: a property of the class, not one lucky vocabulary. Nor is it a finer-lattice artifact: snapping PMT's onsets to the beat grids' resolution still leaves it 67-129 FMD ahead of both (n=500). The effect is distributional; whether it is audible is a separate question, left open by our probe, with a human study pre-registered. Native caption adherence is weak but separable: a lightweight decode-time constraint doubles instrument-F1 (.28 to .60) and Correct-Key (.16 to .35) at no distributional cost. We release the harness, 25+ checkpoints, two corpora (86.6k aligned across caption/MIDI/ABC/audio; 6.25M captioned, the largest for music), and an imprinting diagnostic: published text-to-MIDI systems reproduce their training distribution near-invariant to the caption (7…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.03999v1)
- [PDF](https://arxiv.org/pdf/2608.03999v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/machine-learning
