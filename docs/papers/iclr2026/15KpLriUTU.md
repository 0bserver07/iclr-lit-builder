# PUM-Net: Plastic Unified Memory Network with Associative Interaction for Long-Context State Space Models

**Venue:** iclr2026 (Withdraw)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=15KpLriUTU](https://openreview.net/forum?id=15KpLriUTU)

## Relevance

**LLM score:** 1/3 — Tangential: mentions training cost reduction by avoiding sequence length inflation, but the main contribution is a memory architecture for long-context recall, not energy-efficient training.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
Recent Mamba-family State Space Models (SSMs) leverage linear recurrent dynamics to achieve efficiency in long-sequence modeling. However, their exponential decay kernels inevitably cause rapid forgetting, making it difficult to recall information once sequence lengths far exceed the training horizon. Inspired by advances in Transformer-based architectures such as Native Sparse Attention (NSA), which employ internal chunk memory to alleviate long-term forgetting, we extend Mamba with a chunk-wise internal long-term memory that improves the retrieval of distant context. While this enhances in-context recall, a more fundamental challenge for long-context models is the ability to access and integrate vast external world knowledge without compromising efficiency. Existing retrieval-augmented generation (RAG) approaches attempt to address this by appending retrieved documents to queries, which substantially increases training cost and fails to fully integrate internal and external memory representations. To overcome these limitations, we propose the Plastic Unified Memory Network (PUM-Net), a unified dual-memory architecture that, for the first time, enables joint pre-training over both dynamic internal memory and static, pre-encoded external knowledge. This plastic unification allows external memory to refine internal states during training, enabling bidirectional interaction without inflating sequence length, thereby supporting more effective long-context modeling and achieving substantial improvements across long-range challenging benchmarks.

## Keywords
State Space Model, Long Context, Internal Memory, External Memory
