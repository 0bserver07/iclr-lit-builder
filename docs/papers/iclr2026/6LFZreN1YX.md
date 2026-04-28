# AlignPrune: Robust Dynamic Data Pruning through Loss Trajectory Alignment

**Venue:** iclr2026 (Withdraw)
**Authors:** Huaiyuan Qin, Muli Yang, Gabriel James Goenawan, Kai Wang, Zheng Wang, Peng Hu, Xi Peng, Hongyuan Zhu
**OpenReview:** [https://openreview.net/forum?id=6LFZreN1YX](https://openreview.net/forum?id=6LFZreN1YX)

## Relevance

**LLM score:** 2/3 — The paper advances dynamic data pruning, a technique for efficient training by reducing data usage, which aligns with energy-efficient AI training but does not directly target the Sutro Group's specific named priorities such as data movement, cache-aware ML, or sparse parity.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Existing dynamic data pruning methods often fail under noisy-label settings, as they typically rely on per-sample loss as the ranking criterion. This could mistakenly lead to preserving noisy samples due to their high loss values, resulting in significant performance drop. To address this, we propose AlignPrune, a noise-robust module designed to enhance the reliability of dynamic pruning under label noise. Specifically, AlignPrune introduces the Dynamic Alignment Score (DAS), which is a loss-trajectory-based criterion that enables more accurate identification of noisy samples, thereby improving pruning effectiveness. As a simple yet effective plug-and-play module, AlignPrune can be seamlessly integrated into state-of-the-art dynamic pruning frameworks, consistently outperforming them without modifying either the model architecture or the training pipeline. Extensive experiments on five widely-used benchmarks across various noise types and pruning ratios demonstrate the effectiveness of AlignPrune, boosting accuracy by up to 6.3% over state-of-the-art baselines. Our results offer a generalizable solution for pruning under noisy data, encouraging further exploration of learning in real-world scenarios.

## Keywords
Data Pruning, Dynamic Data Pruning, Efficient Learning
