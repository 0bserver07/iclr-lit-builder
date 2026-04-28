# Quantization with Purpose: Loss-Aware Bit Allocation for Gradient Compression

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0wCTDqkK8I](https://openreview.net/forum?id=0wCTDqkK8I)

## Relevance

**LLM score:** 3/3 — Directly advances energy-efficient training by reducing data movement via loss-aware gradient quantization, a core Sutro Group priority.
**Keyword hits:** `quantization`

## TLDR
(none provided)

## Abstract
Gradient quantization is a critical technique for reducing communication overhead in large-scale distributed training. However, existing methods often employ fixed bit-width quantization or adaptive quantizers optimized with signal-level distortion metrics such as MSE, which poorly correlate with model performance. In this paper, we propose a novel layer-wise bit allocation framework for gradient quantization, formulated under a rate-distortion optimization (RDO) paradigm. Unlike prior approaches, our method introduces a loss-aware distortion metric that directly quantifies the impact of quantization on training loss, enabling task-aligned solution for bit allocation. A key insight of our work is the linear superposition property of cross-layer loss distortion, which we theoretically justify and empirically validate. This property allows us to decouple the original joint optimization problem and efficiently solve it via a Lagrangian optimization algorithm with linear complexity. Extensive experiments across vision and language tasks—using CNNs, ViTs, LSTMs, and Transformers—demonstrate the effectiveness of our approach. Moreover, our method integrates seamlessly with existing gradient compression techniques, yielding consistent performance gains.

## Keywords
Gradient Compression, Rate-Distortion Optimization, Bit Allocation, Quantization
