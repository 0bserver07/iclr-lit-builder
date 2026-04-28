# HOBA: Higher-Order Block-Diagonal Attention Unrolling for Transformer

**Venue:** iclr2026 (Withdraw)
**Authors:** Mafizur Rahman, Lijun Qian
**OpenReview:** [https://openreview.net/forum?id=2tNlroZztK](https://openreview.net/forum?id=2tNlroZztK)

## Relevance

**LLM score:** 2/3 — The paper's main contribution is a sparse attention mechanism (block-diagonal) that reduces computational cost, aligning with the Sutro Group's focus on sparsity and training efficiency.
**Keyword hits:** `knowledge distillation, distillation, sparse`

## TLDR
(none provided)

## Abstract
Transformers with 2D self-attention are powerful but computationally intensive, specifically for long sequences due to their quadratic complexity. Therefore, sparse attention methods attempt to alleviate this cost by limiting attention patterns. However, they often compromise explainability and fail to generalize well to global dependencies. Therefore, we propose Higher-Order Block-Diagonal Attention (HOBA), a novel transformer variant that models triplet interactions utilizing 3D attention tensors and block-diagonal unrolling. HOBA can capture richer patterns within and across blocks while efficiently modeling long-range dependencies without high computational cost. We use knowledge distillation with RoBERTa as the teacher to train the HOBA student model. We evaluate HOBA on five NLP tasks across eight benchmark datasets, comparing it against Full-3D (without block or cross-block), standard 2D attention, and sparse mechanisms including Longformer, BigBird, Local, and Dilated attention. We further isolate the contributions of block structure and higher-order interactions, confirming HOBA’s superiority over both dense and sparse baselines. We also demonstrate that allowing cross-block interaction yields significant accuracy gains by enhancing longrange token dependencies.

## Keywords
Transformers, higher-order attention, NLP benchmarks, sparse attention, cross-block interaction
