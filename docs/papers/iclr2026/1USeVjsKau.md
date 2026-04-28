# ParoQuant: Pairwise Rotation Quantization for Efficient Reasoning LLM Inference

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1USeVjsKau](https://openreview.net/forum?id=1USeVjsKau)

## Relevance

**LLM score:** 1/3 — The paper focuses on post-training quantization for efficient LLM inference, not on training efficiency or training-specific techniques, making it tangential to the Sutro Group's training-centric priorities.
**Keyword hits:** `model compression, low-precision, quantization, kernel`

## TLDR
(none provided)

## Abstract
Post-training quantization (PTQ) compresses the weights and activations of large language models (LLMs) into low-precision representations to reduce memory footprint and accelerate inference. However, the presence of outliers in weights and activations often leads to large quantization errors and severe accuracy degradation, especially in recent reasoning LLMs where errors accumulate across long chains of thought. Existing PTQ methods either fail to sufficiently suppress outliers or introduce significant overhead during inference. In this paper, we propose Pairwise Rotation Quantization (ParoQuant), a PTQ method that combines hardware-efficient and optimizable independent Givens rotations with channel-wise scaling to even out the magnitudes across channels and narrow the dynamic range within each quantization group, effectively addressing the outlier issue. We further co-design the inference kernel to fully exploit GPU parallelism and keep the rotations and scaling lightweight at runtime. Under weight-only quantization, ParoQuant achieves an average 2.4% accuracy improvement over AWQ on reasoning tasks, with less than 10% overhead. ParoQuant also matches the accuracy of state-of-the-art weight-activation quantization methods. This paves the way for more efficient and accurate deployment of reasoning LLMs.

## Keywords
quantization, large language models, model compression
