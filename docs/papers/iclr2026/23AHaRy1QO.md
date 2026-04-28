# Efficient Fine-tuning with Decomposed Foundation Model

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=23AHaRy1QO](https://openreview.net/forum?id=23AHaRy1QO)

## Relevance

**LLM score:** 3/3 — Directly advances memory- and compute-efficient fine-tuning through model decomposition, integrating sparsity and quantization to enable training on constrained hardware, highly relevant to energy-efficient training priorities.
**Keyword hits:** `quantization`

## TLDR
(none provided)

## Abstract
Fine-tuning billion-scale large language models (LLMs) is challenging due to the extremely large model size, particularly in memory-constrained scenarios, even with parameter-efficient fine-tuning (PEFT) and quantization. To address this challenge, we propose a novel method based on the decomposition then fine-tuning (DeFT) paradigm, which effectively decomposes the foundation model and reduces the number of model parameters during fine-tuning, while retaining model quality. DeFT introduces a highly efficient layer importance aware search algorithm for fine-grained model decomposition and successfully repurposes model decomposition for fine-tuning. Additionally, DeFT can seamlessly integrate with PEFT and quantization methods to enhance fine-tuning efficiency further. Extensive experiments on various LLM backbones demonstrate that DeFT achieves comparable or even better performance than the baseline PEFT and quantization methods, while improving both memory efficiency and computation efficiency for fine-tuning. Remarkably, DeFT enables fine-tuning of a 65B model on a consumer GPU with just 24GB of memory, all without relying on offloading strategies, saving significant expenses for purchasing or renting high-end GPUs.

## Keywords
Large Language Model Fine-tuning, Foundation Model Decomposition
