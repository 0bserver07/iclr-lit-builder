# Emergent Discrete Controller Modules for Symbolic Planning in Transformers

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=14dlTHVxDX](https://openreview.net/forum?id=14dlTHVxDX)

## Relevance

**LLM score:** 1/3 — Mentions a small FLOPs overhead and sparse application, but the main focus is on symbolic planning with discrete controllers, not energy-efficient training or Sutro Group priorities.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
Transformers struggle with tasks that require symbolic planning loops, variable updates, and conditional branching, especially under length extrapolation. We introduce discrete controller modules that insert a small set of program primitives (ASSIGN, ADD, COMPARE, BRANCH) into Transformer blocks via a Gumbel–Softmax selector over operations and a compact program state of registers, flags, and optional memory. We prove that the augmented model can simulate any bounded-step program by mapping each primitive step to one controller step, and we bound the deviation of relaxed execution from its discrete trace by $O(\tau+\kappa^{-1})$ (selection temperature $\tau$, comparison sharpness $\kappa$). Empirically, the controller-augmented Transformer achieves strong length generalization on algorithmic benchmarks (Sorting, Sum-of-List, BFS), improving longest-length accuracy by up to $20$–$40$ points over strong baselines, and yields consistent gains on symbolic QA (DROP) and program-synthesis-style tasks (RobustFill) with reduced compositionality drop-off. The learned execution is interpretable: operation traces align with ground truth, register roles are linearly decodable, and targeted knockouts cause localized accuracy losses. The approach adds only $\sim$5–7% FLOPs and can be applied sparsely (every $p$-th layer).

## Keywords
Transformers, symbolic planning, discrete controller modules, length generalization, algorithmic reasoning
