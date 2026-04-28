# Attention and Compression is all you need for Controllably Efficient Language Models

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6rYa2BUnTt](https://openreview.net/forum?id=6rYa2BUnTt)

## Relevance

**LLM score:** 2/3 — The paper's main contribution is an efficient architecture that reduces compute and memory via compression, directly addressing training/inference efficiency and data movement, aligning with Sutro Group's general efficiency focus though not specifically targeting sparse parity, quantization, or local learning.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
The quadratic cost of attention in transformers motivated the development of efficient approaches: namely sparse and sliding window attention, convolutions and linear attention. Although these approaches result in impressive reductions in compute and memory, they often trade-off with quality, specifically in-context recall performance. Moreover, apriori fixing this quality-compute tradeoff in an architecture means being suboptimal from the get-go: some downstream applications require more memory for in-context recall, while others require lower latency and memory. Further, these approaches rely on heuristic choices that artificially restrict attention, or require handcrafted and complex recurrent state update rules, or they must be carefully composed with attention at specific layers to form a hybrid architecture that complicates the design process, especially at scale.

To address above issues, we propose Compress & Attend Transformer (CAT), a conceptually simple architecture employing two simple ingredients only: dense attention and compression. CAT decodes chunks of tokens by attending to compressed chunks of the sequence so far. Compression results in decoding from a reduced sequence length that yields compute and memory savings, while choosing a particular chunk size trades-off quality for efficiency. Moreover, CAT can be trained with multiple chunk sizes at once, unlocking control of quality-compute trade-offs directly at test-time without any retraining, all in a single adaptive architecture.

In exhaustive evaluations on language modeling, in-context recall, and longcontext understanding, a single adaptive CAT model outperforms many existing efficient models including hybrid architectures across varying inference budgets, when appropriately inference costs matched. Further, a single CAT matches dense transformer in language modeling while being 1.4−3$\times$ faster and requiring 2−9$\times$ lower total memory usage.

## Keywords
efficient architecture, attention, compression, adaptive architecture
