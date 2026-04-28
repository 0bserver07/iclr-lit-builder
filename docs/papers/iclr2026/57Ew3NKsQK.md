# Decoupling of Experts: A Knowledge-Driven Architecture for Efficient LLMs

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=57Ew3NKsQK](https://openreview.net/forum?id=57Ew3NKsQK)

## Relevance

**LLM score:** 1/3 — The paper mentions efficiency in scaling but its main contribution is a knowledge-driven architecture with dynamic experts, not directly addressing training efficiency, data movement, sparsity, or hardware-aware methods central to the Sutro Group.
**Keyword hits:** `moe`

## TLDR
(none provided)

## Abstract
Current large language models (LLMs), particularly Mixture-of-Experts (MoE) variants, face challenges in achieving efficient, structured, and interpretable scaling. We introduce the Decoupling of Experts (DoE) architecture, a novel framework that addresses these limitations by grounding computation in a hierarchically organized and dynamically updated knowledge space. Our methodology features a two-stage lifecycle: we first use Latent Dirichlet Allocation (LDA) to build a semantic topic foundation from the training corpus. This knowledge is then integrated into the main LLM, where it is dynamically refined. Critically, we discard traditional, static MoE experts. Instead, the expert entity is a dynamic \textbf{Knowledge Block} synthesized on-the-fly by reusing the Key and Value matrices from the attention computation. We replace the standard load balancer and softmax gating with an \textbf{Attention Gating Control (AGC)} that employs a VAE-based router with a ReLU activation for expert composition. This entire process is optimized with a composite loss function, balancing next-token prediction with a KL-divergence-based expert loss. Our analysis reveals that this architecture induces a remarkable \textbf{heterogeneous specialization} across layers, with some layers differentiating into "science" and "humanities" domains, while others converge on general functions. This demonstrates a learned, hierarchical division of labor, paving the way for a new, more efficient scaling dimension based on the number of structured experts.

## Keywords
DoE, knowledge block, expert decoupling
