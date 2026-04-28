# Beyond Homogeneous Attention: Memory-Efficient LLMs via Fourier-Approximated KV Cache

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4sx3Jzrg5w](https://openreview.net/forum?id=4sx3Jzrg5w)

## Relevance

**LLM score:** 1/3 — Addresses memory efficiency of KV cache in inference, tangentially related to data movement and hardware-aware kernels but not focused on training.
**Keyword hits:** `pruning, kernel, cache`

## TLDR
(none provided)

## Abstract
Large Language Models struggle with memory demands from the growing Key-Value (KV) cache as context lengths increase. Existing compression methods homogenize head dimensions or rely on attention-guided token pruning, often sacrificing accuracy or introducing computational overhead. We propose FourierAttention, a training-free framework that exploits the heterogeneous roles of transformer head dimensions: lower dimensions prioritize local context, while upper ones capture long-range dependencies. By projecting the long-context-insensitive dimensions onto orthogonal Fourier bases, FourierAttention approximates their temporal evolution with fixed-length spectral coefficients. Evaluations on LLaMA models show FourierAttention achieves the best long-context accuracy on LongBench and Needle-In-A-Haystack (NIAH). Besides, a custom Triton kernel, FlashFourierAttention, is designed to optimize memory via streamlined read-write operations, enabling efficient deployment without performance compromise.

## Keywords
Large Language Model, Long-Context LLM, KV cache optimization
