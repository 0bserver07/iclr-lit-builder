# HT-Sparse: Training-Free Query-Guided Head–Token Sparsification for Long-Video Multimodal Inference

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3Oc8Pg7Kij](https://openreview.net/forum?id=3Oc8Pg7Kij)

## Relevance

**LLM score:** 1/3 — The paper proposes training-free inference sparsity for long-video multimodal models, touching on sparsity but not addressing energy-efficient training or data movement in training, making it tangential to the Sutro Group's focus on training efficiency.
**Keyword hits:** `sparsity, sparse, cache`

## TLDR
(none provided)

## Abstract
Long-video multimodal inference is limited by the quadratic cost of dense attention, cumulative KV-cache growth during decoding, and cross-modal interference, while retraining sparsity-aware variants is often impractical. We present HT-Sparse, a training-free, query-guided hierarchical sparsification that performs joint head–token computation to reduce both latency and memory without parameter updates. The method comprises two components executed adaptively across layers: (i) query-conditioned head sparsification, which ranks attention heads via analytically stable saliency statistics to retain the most informative subspaces for the current query; (ii) cross-modal token sparsification, which selects salient visual tokens by query–vision attention, enabling efficient computation and persistent KV-cache savings. We further introduce joint head–token routing in selected layers: top-ranked heads attend to the full visual token set, whereas secondary heads operate on the reduced (selected) set, preserving semantics while amortizing compute and cache. Across long-video benchmarks, HT-Sparse delivers faster inference with reduced end-to-end latency and lower KV-cache memory, while achieving equal or higher accuracy, all on the same pretrained model with no fine-tuning. The approach is model-agnostic and plug-in deployable, offering a flexible route to scalable long-video reasoning.

## Keywords
Long-video multimodal inference, Training-free, query-guided, sparse attention, head–token sparsification
