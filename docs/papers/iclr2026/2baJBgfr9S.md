# HiDivDrop: Vision Token Reduction in MLLMs via Late Injection and Differentiable Top-K

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2baJBgfr9S](https://openreview.net/forum?id=2baJBgfr9S)

## Relevance

**LLM score:** 3/3 — The paper directly advances energy-efficient training by sparsifying visual tokens, reducing data movement and computation in MLLMs.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
The computational cost of Multimodal Large Language Models (MLLMs), driven by the quadratic complexity of processing vision tokens, remains a significant barrier to their widespread adoption. While progressive vision token pruning is a promising solution, we find that its full potential has been unrealized due to two key limitations: it misinterprets the role of shallow layers as being crucial for fusion and employs overly rigid, non-adaptive pruning schedules. To address these flaws, we introduce HiDivDrop, a framework that tailors token pruning to the true hierarchical function of MLLM layers. HiDivDrop incorporates two key innovations: (1) a Late Injection strategy that bypasses passive shallow layers, introducing visual tokens directly where active fusion begins; and (2) a Concave Pyramid Pruning scheme with an Early Exit mechanism that dynamically adjusts the pruning rate throughout the middle and deep layers. This process is optimized via an inter-layer similarity measure and a differentiable top-$k$ operator. Extensive experiments show that HiDivDrop compresses $\sim$90\% visual tokens while matching the original performance and accelerating training by 1.72$\times$. Our work not only sets a new state-of-the-art for efficient MLLM training and inference but also provides valuable insights into the hierarchical nature of multimodal fusion.

## Keywords
MLLMs, Vision Token Pruning, Efficiency and Compression, Interpretability and Analysis
