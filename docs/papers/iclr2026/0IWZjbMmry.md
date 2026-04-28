# LayerDecompose: Exploring weight sharing for Large Language Model Compression

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0IWZjbMmry](https://openreview.net/forum?id=0IWZjbMmry)

## Relevance

**LLM score:** 1/3 — Focuses on post-training compression for deployment, not energy-efficient training or the Sutro Group's named training-efficiency priorities.
**Keyword hits:** `model compression, low-rank, pruning`

## TLDR
(none provided)

## Abstract
Recent advances in large language model (LLM) compression have predominantly focused on pruning and low-rank factorization, leaving weight sharing—despite its success in classical neural network compression—largely unexplored. We introduce LayerDecompose, a novel framework that reduces parameter redundancy by sharing a core weight matrix across transformer layers and augmenting each layer with lightweight, low-rank adapters. Unlike prior SVD- and pruning-based methods, our joint optimization of shared weights and residual adapters achieves a 30% model size reduction while retaining 89% of the original performance on seven standard benchmarks. Experiments on LLaMA and other models demonstrate that LayerDecompose consistently outperforms state-of-the-art baselines. These results highlight the promise of combining weight sharing with low-rank adaptation for efficient, scalable LLM deployment.

## Keywords
Large Language Models (LLMs), Model Compression, Weight Sharing
