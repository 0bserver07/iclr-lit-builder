# Stochastic Layer-wise Learning: Scalable and Efficient Alternative to Backpropagation

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=64f8NQ9Ptj](https://openreview.net/forum?id=64f8NQ9Ptj)

## Relevance

**LLM score:** 3/3 — Proposes a local learning method that eliminates backpropagation, reducing memory and data movement, directly advancing biologically-plausible local learning and energy-efficient training.
**Keyword hits:** `local learning`

## TLDR
(none provided)

## Abstract
Backpropagation underpins modern deep learning, yet its reliance on global gradient synchronization limits scalability and incurs high memory costs. In contrast, fully local learning rules are more efficient but often struggle to maintain the cross-layer coordination needed for coherent global learning. Building on this tension, we introduce Stochastic Layer-wise Learning (SLL), a layer-wise training algorithm that decomposes the global objective into coordinated layer-local updates while preserving global representational coherence.  The method is ELBO-inspired under a Markov assumption on the network, where the network-level objective decomposes into layer-wise terms and each layer optimizes a local objective via a deterministic encoder. The intractable KL in ELBO is replaced by a Bhattacharyya surrogate computed on auxiliary categorical posteriors obtained via fixed geometry-preserving random projections, with optional multiplicative dropout providing stochastic regularization. SLL optimizes locally, aligns globally, thereby eliminating cross-layer backpropagation. Experiments on MLPs, CNNs, and Vision Transformers from MNIST to ImageNet show that the approach surpasses recent local methods and matches global BP performance while memory usage invariant with depth. The results demonstrate a practical and principled path to modular and scalable local learning that couples purely local computation with globally coherent representations.

## Keywords
Local Learning, Representation Learning, Contrastative Learning, ELBO
