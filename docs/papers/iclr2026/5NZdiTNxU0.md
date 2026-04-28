# One-Shot Multi-Label Causal Discovery in High-Dimensional Event Sequences

**Venue:** iclr2026 (Withdraw)
**Authors:** Hugo Math, Robin Schön, Rainer Lienhart
**OpenReview:** [https://openreview.net/forum?id=5NZdiTNxU0](https://openreview.net/forum?id=5NZdiTNxU0)

## Relevance

**LLM score:** 1/3 — The paper mentions efficient parallelized causal discovery on GPUs as a secondary benefit, but the core contribution is causal discovery, not energy-efficient training, data movement, or other Sutro Group priority topics.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
Understanding causality in event sequences where outcome labels such as diseases or system failures arise from preceding events like symptoms or error codes is critical in domains such as healthcare, cybersecurity, and vehicle diagnostics. Yet, existing causal discovery methods struggle to be practical under high-dimensional, sparse sequences involving thousands of event types—a common trait in real-world data. We propose OSCAR, a novel one-shot causal autoregressive discovery method that identifies the Markov Boundaries of each label directly from a single sequence of events. By leveraging two pretrained Transformers as density estimators, OSCAR estimates the conditional mutual information between the current event and future labels given the past sequence, enabling for the first time efficient parallelised causal discovery on GPUs. On a real-world vehicle dataset with 29,100 event types and 474 labels, OSCAR successfully recovers meaningful causal structures where classical algorithms fail to scale, demonstrating a practical path toward interpretable and efficient causal reasoning in complex sequential domains.

## Keywords
event sequence, causal discovery, multi-label causal discovery, autoregressive transformers, markov boundary
