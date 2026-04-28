# LeSTD: LLM Compression via Learning-based Sparse Tensor Decomposition

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0oHaazjMUX](https://openreview.net/forum?id=0oHaazjMUX)

## Relevance

**LLM score:** 1/3 — The paper focuses on post-training compression using sparsity, which is tangential to Sutro Group's emphasis on energy-efficient training; sparsity here serves model compression rather than training efficiency improvements.
**Keyword hits:** `sparsity, low-rank, pruning, sparse`

## TLDR
(none provided)

## Abstract
Large Language Models (LLMs) achieve remarkable success, but their massive parameter counts present significant deployment challenges. Post-training tensor decomposition offers a promising, data-free compression strategy by exploiting structural redundancies within the model weights. However, existing tensor methods face a critical limitation: the dense core tensor bottleneck. While these methods find a shared low-rank basis, the resulting dense core tensor grows polynomially with the chosen ranks, becoming a new storage bottleneck and capping the maximum achievable compression. To overcome this fundamental barrier, we introduce LeSTD (\textbf{Le}arning-based \textbf{S}parse \textbf{T}ensor \textbf{D}ecomposition), a novel two-stage framework for the high-ratio compression of Multi-Head Attention (MHA) blocks. LeSTD first employs an iterative algorithm to identify a high-quality, and shared orthogonal basis that jointly represents all attention heads. Subsequently, it introduces a principled, importance-based pruning algorithm that learns an ultra-sparse core tensor by systematically removing the least salient elements and refitting the remaining ones to preserve model fidelity. By decoupling basis optimization from core sparsification, LeSTD breaks the compression ceiling imposed by the dense core, enabling significantly higher compression ratios than prior methods.

## Keywords
LLM Compression, Post-training Compression, Tucker Decomposition, Sparsity
