# SMixer: Rethinking Efficient-Training and Event-Driven SNNs

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=78glEsQB0v](https://openreview.net/forum?id=78glEsQB0v)

## Relevance

**LLM score:** 3/3 — Directly advances energy-efficient training of spiking neural networks through sparsity (spatial-temporal pruning), aligning with biologically-plausible learning and sparsity priorities.
**Keyword hits:** `energy-efficient, pruning, sparse`

## TLDR
(none provided)

## Abstract
Spiking Neural Networks (SNNs) offer a promising, energy-efficient paradigm for computation, but their practical application is hindered by challenges in architecture design and training costs. For example, Spiking ResNet exhibits relatively low performance, whereas high-performance Spiking Transformers are not truly event driven and cannot be implemented on asynchronous chips. Moreover, the intrinsic time steps and neuron state dynamics result in a substantial computational overhead for training SNNs on GPUs. In response to these problems, we discuss rational architectural design for SNNs and argue that such designs should exhibit three key characteristics: operations fully supported by asynchronous scenarios, low training overhead and competitive performance. In light of this, we adopt the event-driven friendly Spiking Mixer (SMixer) as the foundational architecture and develop a spike feature Spatial-Temporal Pruning (STP) framework with a high pruning ratio and no trainable parameters to reduce the training overhead. Based on a statistical analysis of sparse spike features, STP eliminates redundant spike features across both spatial and temporal dimensions, thereby reducing the input features and computational load during training. It adaptively selects the most salient spike tokens spatially and dynamically constrains neuron firing rates temporally. By leveraging STP and architectural adaptation, SMixer accelerates training while ensuring a fully event-driven characteristics and maintaining competitive performance, offering valuable insights for the design of efficient, event-driven SNNs.

## Keywords
Spiking Neural Network, Efficient Computation, Prune Method
