# Routing Matters in MoE: Scaling Diffusion Transformers with Explicit Routing Guidance

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1w1jCfYM8P](https://openreview.net/forum?id=1w1jCfYM8P)

## Relevance

**LLM score:** 1/3 — MoE is efficiency-related, but the paper focuses on improving expert specialization for vision, not on training efficiency, data movement, sparsity, quantization, or local learning as a main contribution.
**Keyword hits:** `moe`

## TLDR
(none provided)

## Abstract
Mixture-of-Experts (MoE) has emerged as a powerful paradigm for scaling model capacity while preserving computational efficiency. Despite its notable success in large language models (LLMs), existing attempts to apply MoE to Diffusion Transformers (DiTs) have yielded limited gains. We attribute this gap to fundamental differences between language and visual tokens. Language tokens are semantically dense with pronounced inter-token variation, while visual tokens exhibit spatial redundancy and functional heterogeneity, hindering expert specialization in vision MoE. To this end, we present $\textbf{ProMoE}$, an MoE framework featuring a two-step router with explicit routing guidance that promotes expert specialization. Specifically, this guidance encourages the router to $\textit{first}$ partition image tokens into conditional and unconditional sets via conditional routing according to their functional roles, and $\textit{second}$ refine the assignments of conditional image tokens through prototypical routing with learnable prototypes based on semantic content. Moreover, the similarity-based expert allocation in latent space enabled by prototypical routing offers a natural mechanism for incorporating explicit semantic guidance, and we validate that such guidance is crucial for vision MoE. Building on this, we propose a routing contrastive loss that explicitly enhances the prototypical routing process, promoting intra-expert coherence and inter-expert diversity. Extensive experiments on ImageNet benchmark demonstrate that ProMoE surpasses state-of-the-art methods under both Rectified Flow and DDPM training objectives. Code and models will be made publicly available.

## Keywords
Image Generation, Mixture-of-Experts, Diffusion Transformer
