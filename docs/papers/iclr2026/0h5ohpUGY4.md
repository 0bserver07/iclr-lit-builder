# Understanding Dataset Distillation via Spectral Filtering

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0h5ohpUGY4](https://openreview.net/forum?id=0h5ohpUGY4)

## Relevance

**LLM score:** 3/3 — Directly advances energy-efficient training through dataset distillation, which reduces data requirements and speeds up model training, aligning with the group's focus on distillation and efficiency.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
Dataset distillation (DD) has emerged as a promising approach to compress datasets and speed up model training. However, the underlying connections among various DD methods remain largely unexplored. In this paper, we introduce UniDD, a spectral filtering framework that unifies diverse DD objectives. UniDD interprets each DD objective as a specific filter function applied to the eigenvalues of the feature-feature correlation (FFC) matrix to extract certain frequency information of the feature-label correlation (FLC) matrix. In this way, UniDD reveals that the essence of DD fundamentally lies in matching frequency-specific features. Moreover, we characterize the roles of different filters. For example, low-pass filters, \eg, DM and DC, capture blurred patches, while high-pass filters, \eg, MTT and FrePo, prefer to synthesize fine-grained textures and have better diversity. However, existing methods can only learn the sole frequency information as they rely on fixed filter functions throughout distillation. To address this limitation, we further propose Curriculum Frequency Matching (CFM), which gradually adjusts the filter parameter to cover both low- and high-frequency information of the FFC and FLC matrices. Extensive experiments on small-scale datasets, such as CIFAR-10/100, and large-scale ImageNet-1K, demonstrate the superior performance of CFM over existing baselines and validate the practicality of UniDD.

## Keywords
Dataset Distillation, Spectral Filtering
