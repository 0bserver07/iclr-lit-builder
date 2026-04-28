# KDP: Simplifying Representation Dynamics in Kernel Space

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=262LUKGdQn](https://openreview.net/forum?id=262LUKGdQn)

## Relevance

**LLM score:** 1/3 — The paper proposes a model compression method via layer pruning, which yields inference efficiency gains but is not directly about energy-efficient training, data movement, sparsity during training, or other Sutro Group priorities.
**Keyword hits:** `model compression, pruning, kernel`

## TLDR
(none provided)

## Abstract
This paper proposes Kernelized Dynamics Pruning (KDP), a novel layer pruning method from the perspective of simplifying representation dynamics within large language models (LLMs). Motivated by the high similarity between consecutive layer representations, we view the LLM's forward pass as a discrete-time dynamical system. We speculate that this phenomenon indicates the model's internal dynamics have entered a ``slow manifold'', which exhibits computational redundancy. Based on this insight, we project the representations into a kernel space where the complex, non-linear transformation between them is simplified to an approximately linear one. Then, a simple network learns the inverse kernel transformation, thereby enabling the pruning of the entire layer block. Both theoretical analysis and extensive experiments validate the effectiveness of KDP, demonstrating its superiority over existing pruning baselines. Code is available at https://anonymous.4open.science/r/draft-123abc.

## Keywords
Large Language Models, Model Compression, Structured Pruning, Kernel Space
