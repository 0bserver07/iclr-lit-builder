# QuantSparse: Comprehensively Compressing Video Diffusion Transformer with Model Quantization and Attention Sparsification

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4TAG3aQljJ](https://openreview.net/forum?id=4TAG3aQljJ)

## Relevance

**LLM score:** 1/3 — The paper focuses on compressing video diffusion transformers for inference using quantization and attention sparsification, which is tangential to the Sutro Group's core interest in energy-efficient training.
**Keyword hits:** `quantization, second-order, distillation, sparsity, sparse`

## TLDR
(none provided)

## Abstract
Diffusion transformers exhibit remarkable video generation capability, yet their prohibitive computational and memory costs hinder practical deployment. Model quantization and attention sparsification are two promising directions for compression, but each alone suffers severe performance degradation under aggressive compression. Combining them promises compounded efficiency gains, but naive integration is ineffective. The sparsity-induced information loss exacerbates quantization noise, leading to amplified attention shifts. To address this, we propose **QuantSparse**, a unified framework that integrates model quantization with attention sparsification. Specifically, we introduce *Multi-Scale Salient Attention Distillation*, which leverages both global structural guidance and local salient supervision to mitigate quantization-induced bias. In addition, we develop *Second-Order Sparse Attention Reparameterization*, which exploits the temporal stability of second-order residuals to efficiently recover information lost under sparsity. Experiments on HunyuanVideo-13B demonstrate that QuantSparse achieves 20.88 PSNR, substantially outperforming the state-of-the-art quantization baseline Q-VDiT (16.85 PSNR), while simultaneously delivering a **3.68$\times$** reduction in storage and **1.88$\times$** acceleration in end-to-end inference.

## Keywords
Video Generation, Model Quantization, Attention Sparsification
