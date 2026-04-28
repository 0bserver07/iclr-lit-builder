# MSAVQ: Multi-dimensional Sensitivity-Aware Vector Quantization for Ultra-Low-Bit Vision-Language Models

**Venue:** iclr2026 (Desk Reject)
**Authors:** Wang Zhong, Zukang Xu, Xing Hu, Chen Hao, Dawei Yang
**OpenReview:** [https://openreview.net/forum?id=3cM4CCoFpe](https://openreview.net/forum?id=3cM4CCoFpe)

## Relevance

**LLM score:** 2/3 — Quantization is a main contribution, aligning with the low-precision interest, but the paper targets deployment compression rather than energy-efficient training.
**Keyword hits:** `memory bandwidth, quantization`

## TLDR
(none provided)

## Abstract
Vision-Language Models (VLMs) have achieved remarkable progress, but their massive scale severely limits deployment in resource-constrained settings.
Among existing compression strategies, vector quantization (VQ) stands out for its strong representational power under ultra-low bitwidths. 
VQ achieves this by constructing a compact codebook, where weight vectors are mapped to their closest discrete codewords, thereby reducing storage and memory bandwidth requirements while retaining expressive capacity. 
However, applying VQ directly to VLMs faces two fundamental challenges: 
(1) Modality-induced weight heterogeneity.
In VLMs, image and text inputs induce divergent weight distributions, which a unified codebook fails to capture.
(2) Error compensation mismatch from ignoring first-order gradients.
In VLMs, first-order gradients significantly contribute to quantization error, yet conventional VQ methods neglect them, causing biased compensation and accuracy loss
To this end, we propose \textbf{MSAVQ} (Multi-dimensional Sensitivity-Aware Vector Quantization), a framework that addresses these issues with two key components:
(1) Sensitivity-driven structured
mixed-precision quantization, a mixed-precision scheme that allocates bit-widths based on channel sensitivity, combining global and local saliency metrics for fine-grained and interpretable resource distribution. 
(2)Gradient-aware error compensation, a compensation method that explicitly incorporates first-order gradients to address their non-negligible role in VLM quantization errors, with efficient computation enabled by Kronecker and Block-LDL decompositions.
We evaluate MSAVQ on representative VLMs, including LLaVA-onevision, InternVL2, and Qwen2-VL. In 2-bit settings, it consistently surpasses state-of-the-art PTQ methods, achieving up to \textbf{+4.9} higher accuracy (71.4\% vs. 67.0\% on InternVL2-26B). 
These results demonstrate that MSAVQ provides a simple and effective solution for ultra-low-bit quantization of multimodal foundation models, enabling practical deployment under strict resource budgets.

## Keywords
vector quantization, llm, vlm
