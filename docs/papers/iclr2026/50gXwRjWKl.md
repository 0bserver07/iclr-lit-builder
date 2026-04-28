# TEL: A Thermodynamics-Inspired Layer for Adaptive, and Efficient Neural Learning

**Venue:** iclr2026 (Withdraw)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=50gXwRjWKl](https://openreview.net/forum?id=50gXwRjWKl)

## Relevance

**LLM score:** 1/3 — Efficiency is mentioned as a property (minimal overhead, fixed compute budget) but the core contribution is a novel adaptive layer, not a primary focus on energy-efficient training techniques like sparsity, quantization, or data movement reduction.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
We introduce the Thermodynamic Equilibrium Layer (TEL), a neural building block that replaces fixed activations with a short, $K$-step energy-guided refinement. TEL performs $K$ discrete gradient steps on a Gibbs-inspired free energy with a learnable step size and an entropy-driven, adaptable temperature estimated from intermediate activations. This yields nonlinearities that are dynamic yet stable, expose useful per-layer diagnostics (temperature and energy trajectories), and run with a fixed, predictable compute budget. Across a broad suite of tasks, TEL matches or exceeds strong baselines, including MLPs, modern implicit/energy-based layers under compute-matched dimensionality, FLOPs, and parameters. Swapping TEL in place of MLP feed forwards in standard different architectural blocks incurs minimal overhead while consistently improving performance. Together, these results position TEL as a scalable, drop-in alternative for constructing adaptable nonlinearities in deep networks.

## Keywords
Iterative learning, Phsics based architecture, Gibbs free energy, adaptive nonlinearity, Non linear layer
