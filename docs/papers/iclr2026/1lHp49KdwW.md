# UNIFIED MULTI-TEACHER DISTILLATION ACROSS HYBRID NEURAL ARCHITECTURES

**Venue:** iclr2026 (Withdraw)
**Authors:** Wu Ran, Weijia Zhang, ShuYang Pang, JingSheng Liu, Xiaohui Zhang, Yichao Yan, Chao Ma
**OpenReview:** [https://openreview.net/forum?id=1lHp49KdwW](https://openreview.net/forum?id=1lHp49KdwW)

## Relevance

**LLM score:** 2/3 — The paper's main contribution is a multi-teacher distillation method that reduces training data requirements by 1000x, directly addressing resource-constrained training cost, which aligns with energy-efficient training and distillation priorities.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
Multi-teacher distillation has recently garnered attention to compress vision knowledge rooted in multiple vision foundation models into a versatile student. The latest multi-teacher distillation techniques for foundation models typically require 1B of training data, rendering a prohibitive training cost in resource-constrained scenarios. Moreover, these methods usually adopt vanilla feature alignment between the student and multiple teachers, which neglects the heterogeneity between teachers, making them tend to suffer from competition and conflicts among teachers. To address these limitations, we propose a unified framework to transfer knowledge embedded within multiple vision foundation models into both convolution networks (CNNs) and vision Transformers (ViTs) through training on a 1000$\times$ smaller ImageNet-1k dataset. Specifically, we introduce a learnable model token that interacts with visual features across multiple representational spaces. These interactions are mediated through alternating intra-space and inter-space modules, enabling joint feature alignment across diverse source models and architectures. This simple yet effective strategy facilitates unified knowledge transfer from pre-trained Transformers, CNNs, and their combinations—without relying on complex feature-level distillation. Hence, it also establishes an innovative paradigm for cross-architecture distillation. Extensive experiments demonstrate that the resulting model surpasses all its source models in downstream transfer performance, establishing a new sketch for acquiring vision foundation models.

## Keywords
Multi-teacher distillation, knowledge transfer, vision foundation models
