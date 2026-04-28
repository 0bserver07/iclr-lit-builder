# ESSA: Evolutionary Strategies for Scalable Alignment

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1MX3QC0bSH](https://openreview.net/forum?id=1MX3QC0bSH)

## Relevance

**LLM score:** 3/3 — The paper introduces a gradient-free, hardware-friendly alignment method using evolutionary strategies on compressed LoRA parameters and quantized inference, directly advancing low-precision and hardware-aware optimization for training efficiency.
**Keyword hits:** `quantized, low-rank, int8, int4, lora`

## TLDR
(none provided)

## Abstract
Alignment of large language models (LLMs) typically relies on reinforcement learning from human feedback (RLHF) with gradient-based optimizers such as PPO or GRPO. While effective, these methods require complex distributed training, large memory budgets, and careful hyperparameter tuning, all of which become increasingly difficult at billion-parameter scale. We present ESSA, Evolutionary Strategies for Scalable Alignment, a gradient-free framework that aligns LLMs using only forward inference and black-box optimization. ESSA focuses optimization on low-rank LoRA adapters and further compresses their parameter space by optimizing only the singular values from an SVD decomposition of each adapter matrix. This dimensionality reduction makes evolutionary search practical even for very large models and allows efficient operation in quantized INT4 and INT8 inference mode. Across these benchmarks ESSA improves the test accuracy of Qwen2.5-Math-7B by 12.6% on GSM8K and 14.8% on PRM800K, and raises the accuracy of LLaMA3.1-8B on IFEval by 22.5%, all compared with GRPO. In large-scale settings ESSA shows stronger scaling than gradient-based methods: on Qwen2.5-32B for PRM800K it reaches near-optimal accuracy twice as fast on 16 GPUs and six times as fast on 128 GPUs compared with GRPO. These results position evolutionary strategies as a compelling, hardware-friendly alternative to gradient-based LLM alignment, combining competitive quality with substantially reduced wall-clock time and engineering overhead.

## Keywords
evolutionary strategies, large language models, alignment, LoRA, SVD, reinforcement learning from human feedback
