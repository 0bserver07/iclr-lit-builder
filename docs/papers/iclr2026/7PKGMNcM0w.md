# Winner-Take-All Spiking Transformer for Language Modeling

**Venue:** iclr2026 (Withdraw)
**Authors:** Chenlin Zhou, Sihang Guo, Jiaqi Wang, Kaiwei Che, Dongyang Ma, Qingyan Meng, Zhengyu Ma, Yonghong Tian
**OpenReview:** [https://openreview.net/forum?id=7PKGMNcM0w](https://openreview.net/forum?id=7PKGMNcM0w)

## Relevance

**LLM score:** 3/3 — The paper directly advances energy-efficient AI via sparse, spike-driven, softmax-free spiking transformers for language modeling, aligning with sparsity and biologically-plausible learning priorities.
**Keyword hits:** `energy-efficient, sparse`

## TLDR
(none provided)

## Abstract
Spiking Transformers, which combine the scalability of Transformers with the sparse, energy-efficient dynamics of Spiking Neural Networks (SNNs), have achieved strong results in neuromorphic and vision tasks and attracted increasing attention. 
However, existing directly trained spiking transformers primarily focus on vision tasks with encoder-only architectures. In language modeling, convergence relies heavily on softmax-based spiking self-attention, which incurs high energy costs and poses challenges for neuromorphic deployment.
To address this issue, we introduce Winner-Take-All (WTA) mechanisms into spiking transformers and propose two novel softmax-free, spike-driven self-attention modules: WTA Spiking Self-Attention (WSSA) and Causal WTA Spiking Self-Attention (CWSSA). Based on these, we design WTA-based Encoder-only Spiking Transformer (WE-SpikingFormer) for masked language modeling and WTA-based Decoder-only Spiking Transformer (WD-SpikingFormer) for causal language modeling, systematically exploring direct-training-based softmax-free fully spike-driven transformers for natural language processing. 
Extensive experiments on 16 datasets spanning natural language understanding, question-answering tasks, and commonsense reasoning tasks validate the effectiveness of our approach and highlight the promise of spiking transformers for general language modeling and energy-efficient artificial intelligence.

## Keywords
Spiking Transformer, Spiking Neural Networks, Energy Efficiency, Language Modeling
