# When Reasoning Meets Compression: Understanding the Effects of LLMs Compression on Large Reasoning Models

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2za3iNkwXn](https://openreview.net/forum?id=2za3iNkwXn)

## Relevance

**LLM score:** 1/3 — The paper studies post-training compression (quantization, pruning, distillation) effects on reasoning, focusing on interpretation rather than advancing energy-efficient training techniques.
**Keyword hits:** `model compression, quantization, distillation, quantized, pruning`

## TLDR
(none provided)

## Abstract
Compression methods, including quantization, distillation, and pruning, improve the computational efficiency of large reasoning models (LRMs). However, existing studies either fail to sufficiently compare all three compression methods on LRMs or lack in-depth interpretation analysis. In this paper, we investigate how the reasoning capabilities of LRMs are compromised during compression, through performance benchmarking and mechanistic interpretation. To uncover the effects of compression on reasoning performance, we benchmark quantized, distilled, and pruned DeepSeek-R1 models on four reasoning datasets (AIME 2024, FOLIO, Temporal Sequences, and MuSiQue). To precisely locate compression effects on model weights, we adapt difference of means and attribution patching techniques, focusing on the activation of every linear component in compressed LRMs, to interpret fine-grained causal relationships between weights and various reasoning capabilities. This fine-grained interpretation addresses a fundamental question of compression: which weights are the most important for reasoning? Overall, we find dynamically quantized 2.51-bit R1 reaches close-to-R1 performance. With empirical verification, we present three main findings that generalize across both Llama and Qwen: (1) Weight count has a greater impact on LRMs' knowledge memorization than reasoning, highlighting the risks of pruning and distillation; (2) The MLP up projection in the final layer of distilled LRMs is one of the most important components, offering a new perspective on locating critical weights - a fundamental problem in model compression; and (3) Current quantization methods overly compress the final-layer modules and MLP gate projections, so protecting just 2% of all weights that are excessively compressed can raise average accuracy by 6.57%, greatly surpassing the state-of-the-art.

## Keywords
LLMs Compression, LRMs Compression, Quantization, Pruning, Distillation
