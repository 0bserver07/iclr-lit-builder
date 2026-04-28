# Towards Distributed Neural Architectures

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=40sQXprYlm](https://openreview.net/forum?id=40sQXprYlm)

## Relevance

**LLM score:** 3/3 — Directly advances sparsity and data movement efficiency via learned dynamic routing and compute allocation, aligning with Sutro Group's sparse parity and energy-efficient training priorities.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
We introduce and train distributed neural architectures (DNA) in vision and language domains. DNAs are initialized with a proto-architecture that consists of (transformer, MLP, attention, etc.) modules and routers. Any token (or patch) can traverse any series of modules in any order. DNAs are a natural generalization of the sparse methods such as Mixture-of-Experts, Mixture-of-Depths, parameter sharing, etc. Computation and communication patterns of DNA modules are learnt end-to-end during training and depend on the content and context of each token (or patch). These patterns can be shaped by further requirements added to the optimization objective such as compute/memory efficiency or load balancing. We empirically show that (i) trained DNAs are competitive with the dense baselines in both domains and (ii) compute efficiency/parameter sharing can be learnt from data. Next, we analyze the emergent connectivity and computation patterns in the trained DNAs. We find that the paths that tokens take through the models are themselves distributed according to a power-law. We show that some paths (or, equivalently, groups of modules) show emergent specialization. Finally, we demonstrate that models learn to allocate compute and active parameters in an interpretable way.

## Keywords
Distributed Neural Architectures, Dynamic routing, Emergent Specialization, Modular Networks
