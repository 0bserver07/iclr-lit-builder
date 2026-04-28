# Efficient Fine-Tuning of Quantized Models via Adaptive Rank and Bitwidth

**Venue:** iclr2026 (Withdraw)
**Authors:** Changhai Zhou, Shijie Han, Shiyang Zhang, Yuhua Zhou, WEIZHONG ZHANG, Jin Cheng
**OpenReview:** [https://openreview.net/forum?id=1jXc6SHcUV](https://openreview.net/forum?id=1jXc6SHcUV)

## Relevance

**LLM score:** 3/3 — The paper directly advances low-precision/quantization and memory-efficient fine-tuning, aligning with Sutro Group's core priority of energy-efficient training via quantization and hardware-aware techniques.
**Keyword hits:** `model compression, quantization, quantized, lora`

## TLDR
(none provided)

## Abstract
As large language models (LLMs) scale up, model compression is crucial for their deployment on resource-constrained devices. While methods like QLoRA reduce resource demands by combining parameter quantization with LoRA fine-tuning, their use of uniform precision can limit performance by failing to account for layer-wise variations in parameter sensitivity. Recent advances have explored dynamic mixed-precision quantization and adaptive LoRA ranks, but these strategies are typically optimized in isolation. The synergistic integration of these two dimensions remains an unresolved core challenge. To address this, we introduce **QR-Adaptor**, a unified, gradient-free framework that jointly optimizes the per-layer quantization bit-width and LoRA rank. Instead of indirectly minimizing quantization error, QR-Adaptor formulates the task as a discrete, multi-objective optimization problem, directly guided by downstream task performance and memory constraints using a small calibration dataset. Our extensive experiments show that QR-Adaptor consistently establishes a new Pareto frontier, outperforming state-of-the-art quantized fine-tuning methods. Notably, our approach can surpass the performance of a 16-bit LoRA fine-tuned model while operating with a memory footprint comparable to 4-bit models.

## Keywords
Fine-tuning, Mixed Precision, LoRA, Adaptive rank, Multi-objective optimization
