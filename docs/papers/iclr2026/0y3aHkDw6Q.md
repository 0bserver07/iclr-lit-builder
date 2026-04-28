# BDQ: Bidirectional Diagonal Quantization for LLMs

**Venue:** iclr2026 (Withdraw)
**Authors:** Xiusheng Huang, Zhe Li, Lu Wang, Xuanwu Yin, Dong Li, Jun Zhao, Yequan Wang, Emad Barsoum, Kang Liu
**OpenReview:** [https://openreview.net/forum?id=0y3aHkDw6Q](https://openreview.net/forum?id=0y3aHkDw6Q)

## Relevance

**LLM score:** 1/3 — The paper focuses on post-training quantization for inference efficiency, not on energy-efficient training, though it relates to low-precision techniques.
**Keyword hits:** `quantization`

## TLDR
(none provided)

## Abstract
Post-training quantization has emerged as a widely adopted technique for compressing and accelerating the inference of Large Language Models (LLMs). The primary challenges in LLMs quantization stem from activation outliers, which significantly degrade model performance especially at lower bit precision. While recent approaches attempt to mitigate outliers through linear transformations across feature dimensions, our analysis reveals that the transformed weights and activations still exhibit persistent outlier patterns with concentrated magnitude distributions. In this paper, we first model the mathematical relationship between quantization error and outliers, and then introduce a new metric Flatness to quantify the distribution of outliers. Based on this, we derive the theoretical optimal solution with respect to Flatness. Building on these insights, we propose Bidirectional Diagonal Quantization (BDQ), a novel post-training quantization framework that effectively disperses outlier patterns through optimized matrix transformations. BDQ strategically distributes outlier magnitudes across matrix dimensions via learned diagonal operations. Extensive experiments demonstrate that BDQ establishes a new quantization benchmark. It achieves less than 1% accuracy drop in W4A4 quantization on the LLaMA-3-8B model. In the more challenging W2A4KV16 experiment, compared to state-of-the-art approaches, BDQ reduces the performance gap by 39.1% on the DeepSeek-R1-Distill-LLaMA-70B model.

## Keywords
Post-Training Quantization, Flatness, LLMs
