---
title: "Fine-tune video and image models at scale with NVIDIA NeMo Automodel and 🤗 Diffusers"
source: "https://huggingface.co/blog/nvidia/scale-diffusers-finetuning-nemo-automodel"
author: "Hugging Face Blog"
published: "2026-07-17"
created: 2026-07-19
description: "NVIDIA NeMo Automodel + Diffusers integration for production distributed fine-tuning of Hub diffusion models (FLUX, Wan, HunyuanVideo, Qwen-Image) without checkpoint conversion."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/diffusion
  - keyword/multimodal
  - keyword/machine-learning
  - keyword/fine-tuning
---

# Fine-tune video and image models at scale with NVIDIA NeMo Automodel and 🤗 Diffusers

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/nvidia/scale-diffusers-finetuning-nemo-automodel)
- published:: 2026-07-17

## Abstract / Summary
Joint NVIDIA/Hugging Face post on NeMo Automodel bringing production-grade distributed diffusion training to any Diffusers-format Hub model—no checkpoint conversion or model rewrites. Hugging Face native loading/pipelines; parallelism (FSDP2, TP, EP, CP, PP) as config. Recipes cover Wan 2.1/2.2 T2V, FLUX.1/2-dev, HunyuanVideo 1.5, Qwen-Image with full FT and LoRA. Flow-matching objective, latent caching, multiresolution bucketing. Checkpoints round-trip into Diffusers for inference/sharing. Docs and Apache-2.0 code linked from the post.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)
- [NeMo Automodel GitHub](https://github.com/NVIDIA-NeMo/Automodel)
- [Diffusion Fine-Tuning Guide](https://docs.nvidia.com/nemo/automodel/recipes-e2e-examples/diffusion-fine-tuning)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/diffusion #keyword/multimodal #keyword/machine-learning #keyword/fine-tuning
