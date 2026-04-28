# Online Pseudo-Zeroth-Order Training of Neuromorphic Spiking Neural Networks

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6ZietpbPoB](https://openreview.net/forum?id=6ZietpbPoB)

## Relevance

**LLM score:** 3/3 — Directly advances biologically-plausible local learning and neuromorphic hardware-friendly training, reducing data movement by eliminating backpropagation for on-chip energy-efficient SNN training.
**Keyword hits:** `biologically plausible, energy-efficient`

## TLDR
(none provided)

## Abstract
Brain-inspired neuromorphic computing with spiking neural networks (SNNs) is a promising energy-efficient computational approach. However, successfully training deep SNNs in a more biologically plausible and neuromorphic-hardware-friendly way is still challenging. Most recent methods leverage spatial and temporal backpropagation (BP), not adhering to neuromorphic properties. Despite the efforts of some online training methods, tackling spatial credit assignments by alternatives with competitive performance as spatial BP remains a significant problem. In this work, we propose a novel method, online pseudo-zeroth-order (OPZO) training. Our method only requires a single forward propagation with noise injection and direct top-down signals for spatial credit assignment, avoiding spatial BP's problem of symmetric weights and separate phases for layer-by-layer forward-backward propagation. OPZO solves the large variance problem of zeroth-order methods by the pseudo-zeroth-order formulation and momentum feedback connections, while having more guarantees than random feedback. Combining online training, OPZO can pave paths to on-chip SNN training. Experiments on neuromorphic and static datasets with both fully connected and convolutional networks demonstrate the effectiveness of OPZO with competitive performance compared with spatial BP, as well as estimated low training costs.

## Keywords
neuromorphic computing, spiking neural networks, non-backpropagation training, biological plausibility, pseudo-zeroth-order
