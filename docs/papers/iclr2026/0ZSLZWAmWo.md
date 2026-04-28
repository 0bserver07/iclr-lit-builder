# Disentangling Token Dependencies for Efficient Decoding in Diffusion Language Models

**Venue:** iclr2026 (Withdraw)
**Authors:** Qiuhong Shen, Xingyi Yang, Xinyin Ma, Gongfan Fang, Xinchao Wang
**OpenReview:** [https://openreview.net/forum?id=0ZSLZWAmWo](https://openreview.net/forum?id=0ZSLZWAmWo)

## Relevance

**LLM score:** 1/3 — The paper focuses on inference efficiency for diffusion language models via knowledge distillation, which is tangential to the Sutro Group's emphasis on training efficiency, data movement, sparsity, and other training-centric priorities.
**Keyword hits:** `knowledge distillation, distillation`

## TLDR
(none provided)

## Abstract
Diffusion-based large language models (dLLMs) generate text by gradually filling in masked tokens. However, they’re still slow because they usually decode only one or a few tokens per step. Parallel decoding, which unmasks multiple tokens simultaneously, offers a promising way to accelerate generation, but it often degrades output quality when too many tokens are predicted at once. We identify the root cause: unnecessary dependencies between decoded tokens. When multiple tokens are decoded together, the model may incorrectly condition predictions on each other rather than relying solely on the already-generated context. This leads to reduced output quality. To address this, we propose \textbf{Disentangled Decoding}, a training–inference framework that suppresses harmful intra-step dependencies in dLLM parallel decoding. \emph{In training}, we introduce dependency-aware self-distillation. The model learns, in a single forward pass, to reproduce what a sequential two-step decoding would produce. This encourages the model to predict multiple tokens based solely on global context rather than jointly decoded tokens. \emph{At inference}, we introduce Slow-Fast Decoding, a dynamic strategy that tailors parallelism to each token’s dependency on context. We quantify this dependency using Jensen–Shannon Divergence (JSD). Tokens that are highly dependent on the already-generated context are grouped for faster parallel generation; Other tokens are decoded slowly. Together, these components enable stable, high-quality generation of up to five tokens per step. Across four benchmarks, our method achieves up to $3.3\times$ speedup over vanilla greedy decoding, with minimal loss in generation quality. Please see our project page at \url{https://anonymous.4open.science/r/dsquare-dlm}

## Keywords
diffusion language modek, knowledge distillation
