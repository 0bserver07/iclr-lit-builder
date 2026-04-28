# Catalyst: Reveal the Geometry of Pruning by Reshaping Neural Network

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3O8TAbrMKW](https://openreview.net/forum?id=3O8TAbrMKW)

## Relevance

**LLM score:** 2/3 — The paper introduces a novel structured pruning regularization that is a core sparsity technique, directly relevant to model efficiency and compression, a Sutro Group priority.
**Keyword hits:** `model compression, pruning`

## TLDR
(none provided)

## Abstract
Structured pruning aims to reduce the computational cost of neural networks by removing entire filters or channels, but conventional regularization-based approaches suffer from unstable pruning dynamics and magnitude bias.
In particular, commonly-used regularizers such as L1 and Group Lasso exhibit trivial global minima and fail to align with the geometry of pruning-invariant configurations, leading to a tradeoff between sparsification and model integrity.
We propose Catalyst, a novel regularization framework for structured pruning grounded in extended-space optimization and rigorous landscape geometry. Catalyst introduces auxiliary variables to reshape the loss landscape, admitting a nontrivial global minimizer which aligns to the pruning-invariant set, where pruning decisions are lossless by construction. This formulation enables strong regularization without collapsing the model, and induces robust bifurcation dynamics that separate filters into prune-or-preserve groups with wide decision margins.
We provide theoretical analysis of the optimization geometry and bifurcation behavior, and demonstrate empirically that Catalyst achieves stable, magnitude-invariant pruning with superior performance across benchmarks. Our work establishes a principled foundation for structured pruning through geometric regularization and extended-space dynamics.

## Keywords
Structured pruning, regularization, model compression
