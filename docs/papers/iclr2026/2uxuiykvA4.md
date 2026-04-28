# Reduce What You Use: Input‑Aware Matrix‑Multiplication Pruning for LLMs

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2uxuiykvA4](https://openreview.net/forum?id=2uxuiykvA4)

## Relevance

**LLM score:** 1/3 — The paper proposes inference-time pruning for matrix multiplication, tangential to Sutro Group's focus on training efficiency, sparsity during training, or energy-aware training.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Transformer-based language models achieve strong performance but at high computational cost, raising the question of whether their full dimensional capacity is necessary at inference. We introduce Reduced Matrix-Multiplication (RMM), a training-free rule that adaptively prunes feature dimensions on the fly. Given current activations, RMM scores hidden channels with simple norms, retains a controlled fraction, and performs multiplications only within this reduced subspace—yielding deterministic approximations without altering model weights. Applied uniformly across all linear operations, RMM exposes a smooth accuracy–efficiency frontier governed by a single retention ratio. Across models ranging from 1B to 70B parameters and tasks spanning question answering, reasoning, math, coding, summarization, and vision–language benchmarks, RMM achieves substantial cost reductions with minimal accuracy loss. Larger models tolerate more aggressive pruning, highlighting increasing representational redundancy at scale. These findings demonstrate that high-dimensional computations in LLMs can be systematically compressed, offering a simple and general mechanism for controllable accuracy–efficiency tradeoffs

## Keywords
Redundancy, Matrix pruning, Training-free, Large Language Models
