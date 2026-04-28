# FLARE: Fast Low-rank Attention Routing Engine

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5tdICOjjwI](https://openreview.net/forum?id=5tdICOjjwI)

## Relevance

**LLM score:** 3/3 — Proposes an efficient low-rank attention mechanism that reduces compute and memory, avoids materializing large matrices to reduce data movement, uses fused attention for hardware-aware training, and enables training on large 3D meshes on a single GPU, directly advancing data-movement and hardware-aware training priorities.
**Keyword hits:** `low-rank`

## TLDR
(none provided)

## Abstract
The quadratic complexity of self-attention limits its applicability and scalability on long sequences.
We introduce Fast Low-rank Attention Routing Engine (FLARE),
a simplified latent-attention mechanism wherein each attention head encodes $N$ input tokens onto $M \ll N$ latent tokens and immediately deocdes back.
This produces an implicit rank $\leq M$ attention operator using only two cross-attention steps providing a simple and mathematically transparent low-rank formulation of self-attention that can be implemented in $\mathcal{O}(MN)$ time.
Crucially, FLARE eliminates latent-space self-attention and, by expressing both encode and decode steps as fused-attention operations, avoids ever materializing the $M\times N$ projection matrices.
Moreover, by assigning each head independent latent token slices, FLARE realizes multiple parallel low-rank pathways that collectively approximate a richer global attention pattern without sacrificing efficiency.
Empirically, FLARE trains end-to-end on one-million-point unstructured meshes on a single GPU, achieves state-of-the-art accuracy on PDE surrogate benchmarks, and outperforms general-purpose efficient-attention methods on the Long Range Arena suite.
We additionally release a large-scale additive manufacturing dataset to spur further research.

## Keywords
attention mechanisms, low-rank approximation, PDE surrogate modeling, scientific machine learning, point clouds, unstructured meshes, efficient transformers, additive manufacturing, 3D geometry
