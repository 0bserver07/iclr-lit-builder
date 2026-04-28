# PartInfer: Enabling LLM Inference On Edge Devices

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3sbM94O8Ts](https://openreview.net/forum?id=3sbM94O8Ts)

## Relevance

**LLM score:** 1/3 — The paper focuses on LLM inference efficiency via neuron-level sparsity for edge devices, which is tangential to the group's focus on training efficiency.
**Keyword hits:** `model compression, quantization, sparsity, pruning`

## TLDR
(none provided)

## Abstract
Large Language Models (LLMs) have demonstrated remarkable capabilities across a range of Natural Language Processing (NLP) tasks, but their high computational and memory demands pose significant challenges for deployment on resource-constrained edge devices. Existing approaches to model compression and optimization often rely on coarse-grained pruning or quantization, which can compromise accuracy or require re-training and fine-tuning. In this work, we introduce PartInfer, a neuron-level optimization framework that enables efficient LLM inference on edge devices by exploiting the task-specific activation patterns of neurons. By profiling and identifying both task-specific and general-purpose neurons using an offline LLM profiler, PartInfer implements two key optimizations: Partial Loading, which reduces memory footprint by loading only a subset of neurons that were identified to be most important during the offline stage, and Partial Computation, which dynamically computes only the most relevant neurons at runtime. Evaluation across multiple NLP tasks shows that PartInfer achieves significant reductions in memory footprint and computation while preserving task performance, making it a practical step towards enabling LLM deployment on edge devices.

## Keywords
LLMs, LLM inference, deployment of LLMs, LLMs on edge devices, sparsity, edge devices, neuron-level optimization, memory footprint reduction
