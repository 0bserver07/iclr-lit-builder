# One Stone Three Birds: Training-free Core-context-aware Attention for Efficient LLM Prefilling, Decoding, and KV Caching

**Venue:** iclr2026 (Withdraw)
**Authors:** Zeng You, Yaofo Chen, Shuhai Zhang, Zhijie Qiu, Tingyu Wu, Yingjian Li, Yaowei Wang, Mingkui Tan
**OpenReview:** [https://openreview.net/forum?id=0lGVMSAazo](https://openreview.net/forum?id=0lGVMSAazo)

## Relevance

**LLM score:** 1/3 — The paper focuses on inference-time efficiency via training-free sparse attention, tangential to the group's primary emphasis on energy-efficient training methods.
**Keyword hits:** `sparsity, sparse, cache`

## TLDR
(none provided)

## Abstract
The quadratic computational complexity of self-attention poses a critical bottleneck for large language models (LLMs) processing ultra-long contexts. While various sparse attention and KV cache compression methods have been proposed to improve efficiency, they often suffer from limitations such as reliance on fixed patterns, inability to handle both prefilling and decoding stages, or the requirement for additional training. In this paper, we propose Training-free Core-context-aware Attention (TFCA-Attention), a training-free sparse attention mechanism that achieves “one stone three birds”: it unifies acceleration for prefilling, decoding, and KV cache reduction through a consistent sparsity mechanism. TFCA- Attention features an offline calibration phase that determines head-specific sparsity budgets and an online token selection phase that adaptively retains core context tokens using a lightweight redundancy metric. Theoretically, we provide a bounded approximation error guarantee, ensuring long context modeling accuracy. Extensive experiments demonstrate that TFCA-Attention achieves a 2.8× speedup and reduces KV cache by 61% at 128K context length while maintaining performance comparable to full attention across various benchmarks, offering a practical plug-and-play solution for efficient long-context inference.

## Keywords
Large Language Models, Efficient Attention
