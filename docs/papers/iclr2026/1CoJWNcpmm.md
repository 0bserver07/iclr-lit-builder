# You Do Not Fully Utilize Transformer's Representation Capacity

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1CoJWNcpmm](https://openreview.net/forum?id=1CoJWNcpmm)

## Relevance

**LLM score:** 1/3 — The paper mentions efficiency gains (lower perplexity per FLOP) but focuses on representation capacity, not training energy, data movement, sparsity, quantization, or hardware-aware methods central to the Sutro Group.
**Keyword hits:** `flop`

## TLDR
(none provided)

## Abstract
In contrast to RNNs, which compress their history into a single hidden state, Transformers can attend to all past tokens directly. However, standard Transformers rely solely on the hidden state from the previous layer to represent the entire context. We show that this design choice induces representation collapse and degrades performance. To address this issue, we introduce Layer-Integrated Memory (LIMe), a lightweight extension that leverages existing key–value buffers and learns per-head, per-layer routing weights to integrate representations from all previous layers with negligible overhead. Through extensive experiments—including language modeling, synthetic reasoning benchmarks, and very deep architectures—LIMe consistently achieves faster convergence, lower perplexity per FLOP, and substantial accuracy improvements on synthetic tasks while preserving higher value–vector entropy and improved token separability. Finally, our analysis of the learned routing weights reveals systematic reuse of both local and long-distance features, demonstrating how LIMe mitigates collapse, unlocks richer representations without increasing hidden-state size, and points to promising directions for future research.

## Keywords
Transformers, Attention, Representation Collapse, Residual Stream
