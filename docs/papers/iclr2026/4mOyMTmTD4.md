# LUCID-3D: A Lightweight and Compatible Framework for Unified 3D Understanding and Generation

**Venue:** iclr2026 (Withdraw)
**Authors:** Yongwei Chen, Tianyi Wei, Yushi LAN, Zhaoyang Lyu, Shangchen Zhou, Xudong XU, Xingang Pan
**OpenReview:** [https://openreview.net/forum?id=4mOyMTmTD4](https://openreview.net/forum?id=4mOyMTmTD4)

## Relevance

**LLM score:** 1/3 — The paper mentions reducing training cost by leveraging pretrained models as a secondary benefit, but its main contribution is a unified 3D understanding and generation framework, not training efficiency, data movement, sparsity, quantization, or local learning.
**Keyword hits:** `quantization`

## TLDR
(none provided)

## Abstract
The rapid progress of large multimodal models has inspired efforts toward unified frameworks that couple understanding and generation. While such paradigms have shown remarkable success in 2D, extending them to 3D remains largely underexplored. Existing attempts to unify 3D tasks under a single autoregressive (AR) paradigm lead to significant performance degradation due to forced signal quantization and prohibitive training cost. Our key insight is that the essential challenge lies not in enforcing a unified autoregressive paradigm, but in enabling effective information interaction between generation and understanding while minimally compromising their inherent capabilities and leveraging pretrained models to reduce training cost. Guided by this perspective, we present the first unified framework for 3D understanding and generation that combines autoregression with diffusion. Specifically, we adopt an autoregressive next-token prediction paradigm for 3D understanding, and a continuous diffusion paradigm for 3D generation. A lightweight transformer bridges the feature space of large language models and the conditional space of 3D diffusion models, enabling effective cross-modal information exchange while preserving the priors learned by standalone models. Extensive experiments demonstrate that our framework achieves state-of-the-art performance across diverse 3D understanding and generation benchmarks, while also excelling in 3D editing tasks. These results highlight the potential of unified AR+diffusion models as a promising direction for building more general-purpose 3D intelligence. Our code and models will be released.

## Keywords
3D Understanding, 3D Generation, 3D Editing
