# RCStat: A Statistical Framework of Relative Contextualization in Transformers

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3zdoLd2Q93](https://openreview.net/forum?id=3zdoLd2Q93)

## Relevance

**LLM score:** 1/3 — The paper addresses inference-time efficiency via KV-cache compression, which is tangential to the group's focus on training efficiency.
**Keyword hits:** `cache`

## TLDR
(none provided)

## Abstract
Estimating the importance of input tokens and their activations in auto-regressive models is a fundamental requirement in many applications, such as key-value (KV) cache compression and attribution. Prior work computes token importance using attention weights, which are obtained by normalizing the raw attention logits (query-key inner products) with a softmax operation. However, the softmax normalization suppresses the rich information within the attention logits. We introduce RCStat, a statistical framework that harnesses the raw attention logits via Relative Contextualization (RC) -- a random variable measuring contextual influence from one subset of tokens to another. We derive computationally efficient bounds on the expected RC and demonstrate its utility in two applications:  (i) KV compression, where RC‐based adaptive thresholding evicts substantial portions of the KV cache with minimal quality loss in token generation; and (ii) Attribution, where attention heads with high expected RC yield accurate span‐level attribution. Across QA, summarization, and attribution benchmarks, RCStat achieves state-of-the-art performance, improving generation quality by 15–40\% and attribution accuracy by 2–16\%, all without any model retraining.

## Keywords
Large Language Models, Pre-Softmax Analysis, Attention Logits, Relative Contextualization, KV-Compression, Attribution
