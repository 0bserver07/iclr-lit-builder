# ECMNet: Lightweight Semantic Segmentation with Efficient CNN-Mamba Network

**Venue:** iclr2026 (Withdraw)
**Authors:** Feixiang Du, Shengkun Wu, Xiang Wang, Aoxue Ding, Zhongliang Wang, DOU JIABAO
**OpenReview:** [https://openreview.net/forum?id=0YV1iyqz16](https://openreview.net/forum?id=0YV1iyqz16)

## Relevance

**LLM score:** 1/3 — The paper proposes a lightweight segmentation model focusing on inference efficiency (parameter count, FLOPs) rather than energy-efficient training, data movement, sparsity, low precision, or local learning, making it only tangentially relevant.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
In the past decade, Convolutional Neural Networks (CNNs) and Transformers have achieved wide application in semantic segmentation tasks. Although CNNs with Transformer models greatly improve performance, the global context modeling remains inadequate. Recently, Mamba achieved great potential in vision tasks, showing its advantages in modeling long-range dependency. In this paper, we propose a lightweight Efficient CNN-Mamba Network for semantic segmentation, dubbed as ECMNet.  ECMNet combines CNN with Mamba skillfully in a capsule-based framework to address their complementary weaknesses. Specifically, We design a Enhanced Dual-Attention Block (EDAB) for lightweight bottleneck. In order to improve the representations ability of feature, We devise a Multi-Scale Attention Unit (MSAU) to integrate multi-scale feature aggregation, spatial aggregation and channel aggregation. Moreover, a Mamba enhanced Feature Fusion Module (FFM) merges diverse level feature, significantly enhancing segmented accuracy. Extensive experiments on two representative datasets demonstrate that the proposed model excels in accuracy and efficiency balance, achieving 70.6% mIoU on Cityscapes and 73.6% mIoU on CamVid test datasets, with 0.87M parameters and 8.27G FLOPs on a single RTX 3090 GPU platform.

## Keywords
Semantic segmentation, Lightweight, Convolutional neural network, Mamba
