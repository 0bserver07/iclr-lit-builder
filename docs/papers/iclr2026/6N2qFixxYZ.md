# DES-LOC: Desynced Low Communication Adaptive Optimizers for Foundation Models

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6N2qFixxYZ](https://openreview.net/forum?id=6N2qFixxYZ)

## Relevance

**LLM score:** 3/3 — The paper directly advances energy-efficient training by reducing communication costs in distributed adaptive optimizers, a core data movement and optimizer priority for the Sutro Group.
**Keyword hits:** `optimizer, adam`

## TLDR
(none provided)

## Abstract
Scaling foundation model training with Distributed Data Parallel~(DDP) methods is bandwidth-limited.
Existing infrequent communication methods like Local SGD were designed to synchronize model parameters only and cannot be trivially applied to adaptive optimizers due to additional optimizer states.
Heuristic approaches that keep states local or reset them lack guarantees and can be unstable in compute‑efficient batch regimes; conversely, Local Adam synchronizes all states uniformly and is provably convergent but triples communication costs.
We propose Desynced Low Communication Adaptive Optimizers (DES-LOC), a family of optimizers assigning independent synchronization periods to parameters and momenta, enabling lower communication costs while preserving convergence. Our theoretical analysis shows that while parameter synchronization dominates the asymptotic rate in-expectation, high-probability convergence guarantees require at least infrequent synchronization of the second momentum. Furthermore, we prove that more frequent momentum sync permits larger stable step sizes. Experiments on language models of up to 1.7B show that DES-LOC can communicate 170x less than DDP and 2x less than the previous state-of-the-art Local Adam, enabling 1.3x–2.1x wall‑clock speedups over DDP for 1-13B models on 100Gb/s links. Furthermore, unlike previous heuristic methods, DES-LOC is robust to worker failures offering a scalable, efficient, and fault-tolerant solution for foundation model training.

## Keywords
Distributed Training, Foundation Models, Large Language Models, Optimizers, Communication Efficiency, Federated Learning, Distributed Systems, Optimization Theory, Scaling, Robustness
