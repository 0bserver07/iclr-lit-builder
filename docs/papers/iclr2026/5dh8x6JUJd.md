# LoRA in the Right Place: Which Block to Tune in Parameter-Efficient Fine-Tuning?

**Venue:** iclr2026 (Withdraw)
**Authors:** CHI ZHANG, Jingpu Cheng, Qianxiao Li
**OpenReview:** [https://openreview.net/forum?id=5dh8x6JUJd](https://openreview.net/forum?id=5dh8x6JUJd)

## Relevance

**LLM score:** 1/3 — The paper focuses on parameter-efficient fine-tuning placement for improving adaptation performance, with efficiency as a secondary benefit, but it does not directly address energy-efficient training, data movement, sparsity, quantization, or hardware-aware methods as a main contribution.
**Keyword hits:** `low-rank, lora`

## TLDR
(none provided)

## Abstract
Are all blocks equally important in parameter-efficient fine-tuning? This fundamental question underlies almost every PEFT method, yet decisions about where to insert tunable parameters are often based on convention or ad hoc heuristics. In this work, we revisit this design decision by exploring the theoretical ground behind this choice, with the goal of developing a rigorous understanding of block-level placement within the PEFT paradigm. Starting from a simple scalar example, we show how perturbations in smaller blocks can be amplified through interactions with larger ones, and then extend this reasoning to matrices using norm-based analysis. Our results further reveal that the softmax operation tends to suppress updates to queries and keys, suggesting that value and output blocks should be prioritized. For tasks that rely on class tokens, we find that tuning the output block often outperforms the traditional emphasis on the value block. Importantly, this block-selection principle generalizes beyond the standard LoRA to other PEFT variants such as DoRA and AdaLoRA, underscoring its broad applicability. We validate these insights with extensive experiments across architectures, pretrained models, rank settings, and downstream benchmarks. Overall, our findings establish block selection as a key factor in PEFT and offer principled, empirically grounded strategies for improving both efficiency and effectiveness in model adaptation.

## Keywords
Parameter-Efficient Fine-Tuning, Low-rank Adaptation
