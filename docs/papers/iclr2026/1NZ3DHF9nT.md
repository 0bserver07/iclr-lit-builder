# Fast-dLLM v2: Efficient Block-Diffusion LLM

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1NZ3DHF9nT](https://openreview.net/forum?id=1NZ3DHF9nT)

## Relevance

**LLM score:** 1/3 — The paper primarily contributes to inference efficiency through block diffusion and hierarchical caching, with a tangential mention of reduced fine-tuning data; it does not focus on energy-efficient training, data movement, sparsity, low-precision, or local learning as main contributions.
**Keyword hits:** `cache`

## TLDR
(none provided)

## Abstract
Autoregressive (AR) large language models (LLMs) have achieved remarkable performance across a wide range of natural language tasks, yet their inherent sequential decoding limits inference efficiency. In this work, we propose Fast-dLLM v2, a carefully designed block diffusion language model (dLLM) that efficiently adapts pretrained AR models into dLLMs for parallel text generation—requiring only ∼1B tokens of fine-tuning. This represents a 500× reduction in training data compared to full-attention diffusion LLMs such as Dream (580B tokens), while preserving the original model’s performance. Our approach introduces a novel training recipe that combines a block diffusion mechanism with a complementary attention mask, enabling blockwise bidirectional context modeling without sacrificing AR training objectives. To further accelerate decoding, we design a hierarchical caching mechanism: a block-level cache that stores historical context representations across blocks, and a sub-block cache that enables efficient parallel generation within partially decoded blocks. Coupled with our parallel decoding pipeline, Fast-dLLM v2 achieves up to 2.5× speedup over standard AR decoding without compromising generation quality. Extensive experiments across diverse benchmarks demonstrate that Fast-dLLM v2 matches or surpasses AR baselines in accuracy, while delivering state-of-the-art efficiency among dLLMs—marking a significant step toward the practical deployment of fast and accurate LLMs. Code and model will be publicly released.

## Keywords
Diffusion LLM, Efficient AI
