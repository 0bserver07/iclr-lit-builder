# PRKV:Page Restruct KV Cache for High Accuracy and Efficiency LLM Generation

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7FM0GBFhe5](https://openreview.net/forum?id=7FM0GBFhe5)

## Relevance

**LLM score:** 1/3 — The paper focuses on inference efficiency through KV cache optimization, tangentially related to data movement and caching but not to training efficiency or Sutro Group's training-centric priorities.
**Keyword hits:** `sparse, cache`

## TLDR
(none provided)

## Abstract
As the key-value(KV) cache size scales with context length, accessing large KV
cache each step and substantial GPU memory demand challenge us to deploy
LLMs with long contexts.Various sparse attention methods have been proposed
and offloading-based KV retrieval preserves entire KV cache in CPU memory
and dynamically retrieves most relevant KV pairs for each decoding step, which
performs higher quality and effectively reduces GPU memory consumption than
other line works. However, exiting KV retrieval performs page-level to reduce
estimation overhead, which introduces inaccurate KV selection and significant re-
trieval overhead. We propose PRKV, a framework that both-optimizes algorithm
and system for page-level KV retrieval with KV offloading. On the algorithm side,
PRKV introduces hybrid KV selection that combines both static and dynamic KV
selection strategies. On the system side, PRKV employs contiguous memory in-
dexing and batched transfer optimizations to improve retrieval efficiency. Exper-
iments demonstrate that PRKV improve accuracy across various scenarios and
models, delivering up to 6.75× speedup compared to SOTA KV retrieval methods.

## Keywords
Long-Context LLM Inference, KV Cache Optimization
