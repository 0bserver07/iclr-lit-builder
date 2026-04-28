# Generalization and Scaling Laws for Mixture-of-Experts Transformers

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=57D4Uaiiyi](https://openreview.net/forum?id=57D4Uaiiyi)

## Relevance

**LLM score:** 2/3 — The paper's main contribution is theoretical scaling laws and generalization bounds for sparse (MoE) transformers, explicitly analyzing the efficiency tradeoff between active capacity and routing overhead.
**Keyword hits:** `mixture of experts, sparsity, sparse, moe`

## TLDR
(none provided)

## Abstract
We develop a theory of generalization and scaling for Mixture-of-Experts (MoE) Transformers that cleanly separates \emph{active} per-input capacity from \emph{routing} combinatorics. Conditioning on fixed routing patterns and union-bounding across them, we obtain a sup-norm covering-number bound whose metric entropy scales with the active parameter budget and incurs a MoE-specific overhead. Combining this with a standard ERM argument for squared loss we provided a generalization bound under a $d$-dimensional manifold model and $C^\beta$ targets, showing that approximation and estimation trade off in the same way as in dense networks once active parameters are counted appropriately. We further prove a constructive approximation theorem for MoE architectures, demonstrating that accuracy can be improved either by scaling active capacity or by increasing the number of available experts, with the better of the two mechanisms prevailing. From these results we derive neural scaling laws, covering model scaling, data scaling and compute–optimal tradeoffs.
The theory highlights that enlarging the expert pool at fixed sparsity influences performance only through a mild logarithmic routing term, whereas increasing active capacity per input drives the main gains in generalization and approximation. These insights provide principled guidance for the design of efficient sparse Transformer systems and clarify the fundamental tradeoffs underlying their empirical scaling behavior.

## Keywords
mixture of experts, scaling laws, llm, Sparse Transformers, Generalization bounds
