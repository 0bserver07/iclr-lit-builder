# Efficient Resource-Constrained Training of Transformers via Subspace Optimization

**Venue:** iclr2026 (Oral)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0nvQ5kHXf4](https://openreview.net/forum?id=0nvQ5kHXf4)

## Relevance

**LLM score:** 3/3 — Directly advances energy-efficient training by reducing memory and compute via subspace optimization for on-device transformer training.
**Keyword hits:** `low rank, flops`

## TLDR
(none provided)

## Abstract
As AI increasingly shapes daily life, energy consumption and data privacy have become pressing concerns. On-device learning trains models directly on edge devices, cutting energy consumption and safeguarding data privacy. However, the expanding scale of modern neural networks creates a major obstacle for on-device training. Although prior work has concentrated on compact convolutional architectures, we instead apply subspace-based training to transformer models. Motivated by the idea that a model's essential information lies in a fixed subspace, we introduce Weight-Activation Subspace Iteration (WASI), a method that mitigates the memory bottleneck of backpropagation and boosts inference efficiency in transformer models by restricting training to this subspace. Our results demonstrate that WASI maintains accuracy comparable to vanilla training while reducing memory usage by up to $62\times$ and computational cost (FLOPs) by up to $2\times$. On a Raspberry Pi 5, WASI achieves roughly $1.4\times$ faster training and inference than vanilla training. The code is available at https://github.com/Le-TrungNguyen/ICLR2026-WASI.git.

## Keywords
Deep Learning, Computer Vision, Compression, Low rank
