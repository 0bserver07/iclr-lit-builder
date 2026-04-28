# A Mathematical Framework for the Hierarchical Analysis of Neural Networks

**Venue:** iclr2026 (Desk Reject)
**Authors:** Hossein Mobahi, Peter Bartlett
**OpenReview:** [https://openreview.net/forum?id=5ls9sq3Tv2](https://openreview.net/forum?id=5ls9sq3Tv2)

## Relevance

**LLM score:** 1/3 — Tangentially relevant via model compression, but the core contribution is a mathematical framework for hierarchical analysis and representation of trained networks, not directly advancing energy-efficient training or sparsity techniques.
**Keyword hits:** `model compression`

## TLDR
(none provided)

## Abstract
We introduce a computational framework for analyzing and representing neural networks in a way that is both structurally aware and hierarchical. We begin by developing two general-purpose, mathematically-grounded tools for the pairwise analysis of neurons. First, we introduce Structural Component Analysis (SCA) and prove it finds the optimally disentangled orthonormal basis for the joint input-output weight space. First, Structural Component Analysis (SCA) finds a maximally disentangled orthonormal basis for the joint input-output weight space. Second, we formalize the Gated Interaction Decomposition (GID) provides a generative, and generally oblique, basis that explains how the coupling between input and output weights arises from an interpretable multiplicative gating mechanism. We then present the Hierarchical Encoding via Reversible Merging (HERM) framework, which leverages GID as a core operator to iteratively and losslessly merge pairs of neurons, thereby transforming a trained network into a compressed skeletal representation and a sequence of recovery instructions. This process reveals a meaningful functional hierarchy of the network's learned knowledge. Our theoretical approach provides a new lens for understanding and manipulating neural networks, and we illustrate its potential through proof-of-concept applications in elastic fine-tuning, dynamic architecture design, and model compression.

## Keywords
Hierarchical Merging, Structural Disentanglement, Hierarchical Representation, Interpretability
