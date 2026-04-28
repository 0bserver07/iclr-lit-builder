# Rapid Training of Hamiltonian Graph Networks Using Random Features

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2T4KxtDquV](https://openreview.net/forum?id=2T4KxtDquV)

## Relevance

**LLM score:** 3/3 — Proposes a gradient-descent-free training method achieving 150-600x speedup, directly advancing training efficiency and alternative optimizers.
**Keyword hits:** `adam`

## TLDR
(none provided)

## Abstract
Learning dynamical systems that respect physical symmetries and constraints remains a fundamental challenge in data-driven modeling. Integrating physical laws with graph neural networks facilitates principled modeling of complex N-body dynamics and yields accurate and permutation-invariant models. However, training graph neural networks with iterative, gradient-descent-based optimization algorithms (e.g., Adam, RMSProp, LBFGS) often leads to slow training, especially for large, complex systems. In comparison to 15 different optimizers, we demonstrate that Hamiltonian Graph Networks (HGN) can be trained 150-600× faster - but with comparable accuracy - by replacing iterative optimization with random feature-based parameter construction. We show robust performance in diverse simulations, including N-body mass-spring and molecular dynamics systems in up to $3$ dimensions and 10,000 particles with different geometries, while retaining essential physical invariances with respect to permutation, rotation, and translation. Our proposed approach is benchmarked using a NeurIPS 2022 Datasets and Benchmarks Track publication to further demonstrate its versatility. We reveal that even when trained on minimal 8-node systems, the model can generalize in a zero-shot manner to systems as large as 4096 nodes without retraining. Our work challenges the dominance of iterative gradient-descent-based optimization algorithms for training neural network models for physical systems.

## Keywords
Graph neural networks, physics-informed machine learning, random feature methods, gradient-descent-free training, Hamiltonian neural network
