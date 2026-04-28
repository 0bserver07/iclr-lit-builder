# DeCoP: Enhancing Self-Supervised Time Series Representation with Dependency Controlled Pre-training

**Venue:** iclr2026 (Withdraw)
**Authors:** Yuemin Wu, Zhongze Wu, Xiu Su, Feng Yang, Hongyan Xu, Xi Lin, Wenti Huang, Shan You, Chang Xu
**OpenReview:** [https://openreview.net/forum?id=71GdLqicyH](https://openreview.net/forum?id=71GdLqicyH)

## Relevance

**LLM score:** 1/3 — The paper reduces FLOPs as a side benefit, but its core contribution is time-series representation learning, not directly advancing energy-efficient training, data movement, sparsity, low precision, or local learning.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
Modeling dynamic temporal dependencies is a critical challenge in time series pre-training, which evolve due to distribution shifts and multi-scale patterns. This temporal variability severely impairs the generalization of pre-trained models to downstream tasks. Existing frameworks often adopt uniform instance-level normalization, which overlooks patch-specific characteristics, and model dependencies at a single scale, failing to capture complex temporal variations. To address these limitations, we propose DeCoP, a Dependency Controlled Pre-training framework that explicitly models dynamic, multi-scale dependencies by simulating evolving inter-patch dependency. DeCoP first introduces Instance-wise Patch Normalization (IPN) to mitigate distributional shifts while preserving the unique characteristics of each patch, creating a robust foundation for representation learning. Building on this, a hierarchical Dependency Controlled Learning (DCL) strategy explicitly models inter-patch dependencies across multiple temporal scales within the latent space. This is complemented by a global Instance-level Contrastive Module (ICM), which enhances generalization by learning instance-discriminative representations from time-invariant positive pairs. DeCoP achieves state-of-the-art results on ten datasets, improving MSE by 3% on ETTh1 over PatchTST using only 37% of the FLOPs.

## Keywords
Time series analysis, self-supervised learning
