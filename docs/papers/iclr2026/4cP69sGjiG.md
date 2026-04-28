# Training-time Selection of Linear Vs. Softmax Attention in Layer-based Hybrid Transformers

**Venue:** iclr2026 (Withdraw)
**Authors:** Amir Hossein Mobasheri, Eugene Zailer, Hirotaka Tamura, Yasuhiro Watanabe, Ali Sheikholeslami
**OpenReview:** [https://openreview.net/forum?id=4cP69sGjiG](https://openreview.net/forum?id=4cP69sGjiG)

## Relevance

**LLM score:** 1/3 — The paper addresses inference-time memory efficiency (KV-cache reduction) via layer selection during training, which is tangentially related to data movement and resource usage but does not focus on training efficiency, sparsity, quantization, or local learning.
**Keyword hits:** `cache`

## TLDR
(none provided)

## Abstract
Given a prompt of initial length $M$ to generate $N$ tokens, the current transformer-based LLMs’ memory requirement grows with $\mathcal{O}(M + N)$, while the inference time grows with $\mathcal{O}(MN + N^2)$. While these models have achieved remarkable results across various tasks, their rapid growth rates set upper limits for enhancing the accuracy of the output via increasing the context length due to memory size constraints and time requirements. Linear attention mechanisms offer $\mathcal{O}(N)$ time and constant memory complexity but fall short in some language modeling tasks, especially when the softmax-attention is using the full context. A natural direction is to design hybrid models that combine the strengths of both approaches. In this work, we propose a training-based method for constructing such hybrid models. This method aims to find the optimal layer-based hybrid configuration of a transformer given a maximum tolerable incremental loss. The method aims to replace any softmax attention block with its linear counterpart, so long as it does not incur additional loss beyond a desirable tolerable limit. We evaluate our hybrid models on various language-modeling benchmarks. The result shows that the hybrid models obtained by this method, in some cases, can cut the LLM's total context cache peak memory usage by up to 40 \% while affecting the accuracy minimally (increasing perplexity by 1\%). Furthermore, we observe that our method of training, in some cases, even results in a reduction of the task-specific loss (e.g., cross-entropy) compared to an all softmax-attention configuration. Therefore, using the proposed method not only makes the model more efficient in terms of memory usage and compute intensity but also increases the accuracy, i.e., reduces perplexity. We show that early and final layers can usually be replaced with linear attention layers, while the mid layers must preserve softmax attention, and the exact pattern differs from dataset to dataset.

## Keywords
LLM, Transformer, Attention, Hybrid, Language-modeling, Efficient LLM, Linear Attention, KV-cache
