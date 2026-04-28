# BoundaryDPT: Pushing the Boundaries of Depth Pruning for Vision Transformers

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=71P7ZaKnaO](https://openreview.net/forum?id=71P7ZaKnaO)

## Relevance

**LLM score:** 1/3 — The paper focuses on inference-time speedup via depth pruning, not energy-efficient training or data-movement optimizations during training.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
While prior studies have successfully compressed vision Transformers (ViTs) through various pruning techniques, most have concentrated on width pruning to achieve significant reductions in model size. Depth pruning, which involves the removal of entire layers from a ViT, is notoriously difficult for accuracy recovery, although depth pruning usually leads to higher speedups of compressed ViTs. Consequently, existing joint approaches that incorporate both width and depth pruning have exhibited limited acceleration ratios due to the inefficiencies of previous depth pruning methods.

To tackle the challenges in depth pruning, this work introduces BoundaryDPT, a novel depth pruning method by targeting redundancy of both attention layers and non-linearity within ViTs. To the 
best of our knowledge, we are the first to propose the pruning of activation function layers in ViTs. By reducing the redundancy of nonlinearity, instead of directly targeting linear layers in ViTs, the depths of ViTs are naturally reduced without incurring dimension mismatch. Moreover, we present a two-stage joint pruning method designed to address the heterogeneity of attention layers and activation function layers.

Comprehensive experiments on ImageNet1k, CIFAR-100, and ADE20K have validated our methods. Firstly, BoundaryDPT achieves a 1.58$\times$ speedup for DeiT-B while maintaining accuracy, and a 1.39$\times$ speedup for DeiT-S with nearly lossless accuracy degradation. Furthermore, when combined with width pruning (referred to as BoundaryDPT+), our method sets a new state-of-the-art record in ViT pruning. For instance, BoundaryDPT+ enhances the acceleration ratio from 4.24$\times$ to 5.19$\times$ for the Isomorphic-Pruning-2.6G configuration while maintaining near-lossless accuracy, establishing new benchmarks in extreme ViT compression.

## Keywords
Depth pruning, Activation function pruning, Practical speedups, Transformer compression
