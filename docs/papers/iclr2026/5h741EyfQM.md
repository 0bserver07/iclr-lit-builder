# A Brain-Inspired Gating Mechanism Unlocks Robust Computation in Spiking Neural Networks

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5h741EyfQM](https://openreview.net/forum?id=5h741EyfQM)

## Relevance

**LLM score:** 1/3 — The paper mentions SNNs as energy-efficient but focuses on noise robustness via a biologically-inspired gating mechanism, tangential to the Sutro Group's emphasis on training efficiency, data movement, or hardware-aware methods.
**Keyword hits:** `energy-efficient`

## TLDR
(none provided)

## Abstract
While spiking neural networks (SNNs) provide a biologically inspired and energy-efficient computational framework, their robustness and the dynamic advantages inherent to biological neurons remain significantly underutilized owing to oversimplified neuron models. In particular, conventional leaky integrate-and-fire (LIF) neurons often omit the dynamic conductance mechanisms inherent in biological neurons, thereby limiting their capacity to cope with noise and temporal variability. In this work, we revisit dynamic conductance from a functional perspective and uncover its intrinsic role as a bio-inspired gating mechanism that modulates information flow. Building on this insight, we introduce the Dynamic Gated Neuron~(DGN), a novel spiking unit in which membrane conductance evolves in response to neuronal activity, enabling selective input filtering and adaptive noise suppression. We provide a theoretical analysis showing that DGN possess enhanced stochastic stability compared to standard LIF models, with dynamic conductance intriguingly acting as a disturbance rejection mechanism. DGN-based SNNs demonstrate superior performance across extensive evaluations on anti-noise tasks and temporal-related benchmarks such as TIDIGITS and SHD, consistently exhibiting excellent robustness. To the best of our knowledge, for the first time, our results establish bio-inspired dynamic gating as a key mechanism for robust spike-based computation, providing not only theoretical guarantees but also strong empirical validations. This work thus paves the way for more resilient, efficient, and biologically inspired spiking neural networks.

## Keywords
Spiking Neural Networks (SNNs), Dynamic Gated Neurons, Noise Robustness, Brain-Inspired Computing
