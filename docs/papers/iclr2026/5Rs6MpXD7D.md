# Scaling Weisfeiler–Leman Expressiveness Analysis to Massive Graphs with GPUs

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5Rs6MpXD7D](https://openreview.net/forum?id=5Rs6MpXD7D)

## Relevance

**LLM score:** 1/3 — The paper accelerates a graph algorithm on GPUs but does not focus on energy-efficient AI training, data movement, sparsity, quantization, or local learning.
**Keyword hits:** `cuda`

## TLDR
(none provided)

## Abstract
The Weisfeiler–Leman (WL) test is a cornerstone for analyzing the expressiveness of Graph Neural Networks, but computing its stable coloring at scale has remained a bottleneck. Classical refinement algorithms are inherently sequential and, despite optimal asymptotic complexity, do not exploit modern massively parallel hardware. Moreover, the problem is P-complete, suggesting limited parallelizability in the worst case. We show that these theoretical barriers do not preclude practical scalability. We obtain a linear-algebraic view of stable colorings by reformulating WL refinement as repeated matrix–vector multiplications. Building on this, we introduce two key contributions: (i) a randomized refinement algorithm with tight probabilistic guarantees, and (ii) a batching method that enables the analysis of stable colorings on subgraphs while preserving global correctness. This approach maps directly to GPU-efficient primitives. In numerical experiments, our CUDA implementation delivers up to ~24x speedups over classical CPU-based partition refinement and, for the first time, successfully computes stable colorings on web-scale graphs with over 30 billion edges, where CPU baselines time out or fail.

## Keywords
Weisfeiler-Leman Test (1-WL)  Computation, Randomized Parallel Algorithm, Linear Algebra Characterization
