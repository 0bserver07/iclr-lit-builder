# Vulnerability-Aware Parameter-Efficient Fine-Tuning for Enhanced Adversarial Robustness

**Venue:** iclr2026 (Withdraw)
**Authors:** Abhinab Acharya, Yuansheng Zhu, Dayou Yu, Qi Yu, Xumin Liu
**OpenReview:** [https://openreview.net/forum?id=5TitVYbQQ2](https://openreview.net/forum?id=5TitVYbQQ2)

## Relevance

**LLM score:** 1/3 — The paper uses parameter-efficient fine-tuning (PEFT) for adversarial robustness, but the main contribution is not advancing training efficiency, data movement, sparsity, quantization, or other Sutro Group priorities.
**Keyword hits:** `pruning, lora`

## TLDR
(none provided)

## Abstract
Pre-trained foundation models (PTMs) that undergo standard pre-training can be efficiently finetuned for downstream tasks using parameter-efficient fine-tuning (PEFT) methods. However,  these models remain highly vulnerable to adversarial perturbations. Existing studies often distribute PEFT parameters uniformly across layers, which overlooks the varying importance of each layer. In this work, we systematically analyze the adversarial robustness of PEFT strategies and introduce a novel vulnerability score, a computationally efficient gradient-based measure that identifies which layers and components are most susceptible to adversarial attacks. Guided by this score, we design robustness-aware PEFT methods: LoRA High, which concentrates parameters in the most vulnerable layers, and LoRA+Adapter, which assigns LoRA to the attention component and adapters to the feed-forward component. Extensive adversarial-training experiments across four real-world image classification datasets show that these targeted PEFT designs consistently outperform vanilla PEFT methods. Post-adversarial finetuning analysis with pruning-style attribution score confirms that strategically protecting vulnerable parts of the backbone is key to robustness in PEFT.

## Keywords
Adversarial robustness, parameter-efficient fine-tuning
