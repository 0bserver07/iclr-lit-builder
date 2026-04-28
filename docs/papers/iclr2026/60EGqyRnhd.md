# Spiking Graph Predictive Coding

**Venue:** iclr2026 (Withdraw)
**Authors:** Jing Ren, Jiapeng Du, Bowen Li, Ziqi Xu, Hong Jia, Suyu Ma, Xiwei Xu, Feng Xia
**OpenReview:** [https://openreview.net/forum?id=60EGqyRnhd](https://openreview.net/forum?id=60EGqyRnhd)

## Relevance

**LLM score:** 1/3 — Efficiency is mentioned as a side benefit of event-driven spiking computation, but the paper's main contribution is robust calibration and OOD generalization via local predictive coding, not advancing training efficiency or Sutro Group's specific priorities like data movement, cache-awareness, or sparse parity.
**Keyword hits:** `predictive coding`

## TLDR
(none provided)

## Abstract
Graph Neural Networks (GNNs) have shown strong performance on structured data, but they often suffer from poor calibration and limited generalisation under out-of-distribution (OOD) data, which poses a critical challenge for trustworthy graph learning in real-world applications. In contrast, spiking neural networks (SNNs) and predictive coding (PC) provide biologically grounded mechanisms for event-driven computation and local error correction, which naturally promote robustness and calibrated uncertainty. Inspired by these principles, we propose SpIking GrapH predicTive coding (SIGHT), a framework that integrates PC dynamics with spiking computation for graph learning. SIGHT preserves the architectural flexibility of modern GNNs while replacing global backpropagation with local, spike-driven error correction, yielding learning dynamics that are inherently robust to distribution shifts. Experiments on five graph datasets with two types of OOD scenarios show that SIGHT delivers competitive predictive accuracy, better-calibrated uncertainty, and stronger OOD detection than standard GNNs. Beyond accuracy, the error-driven spiking dynamics provide natural explanations for uncertainty, and the event-driven computation makes SIGHT attractive for deployment on power-constrained hardware, highlighting its potential as a principled and efficient alternative for robust graph learning.

## Keywords
Graph Neural Networks, Spiking Neural Networks, Predictive Coding, Calibration, OOD generalisation, Robustness
