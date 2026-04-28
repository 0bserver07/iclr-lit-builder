# Dataset Distillation via Committee Voting

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1dMsKsfwJ1](https://openreview.net/forum?id=1dMsKsfwJ1)

## Relevance

**LLM score:** 3/3 — Directly advances efficient training through dataset distillation, a core Sutro Group priority, reducing computational resources and energy consumption.
**Keyword hits:** `distillation, green ai`

## TLDR
(none provided)

## Abstract
Dataset distillation aims to synthesize a smaller, representative dataset that preserves the essential properties of the original data, enabling efficient model training with reduced computational resources. Prior work has primarily focused on improving the alignment or matching process between original and synthetic data, or on enhancing the efficiency of distilling large datasets. In this work, we introduce $\bf C$ommittee $\bf V$otingfor $\bf D$ataset $\bf D$istillation (CV-DD), a novel and orthogonal approach that leverages the collective wisdom of multiple models or experts to create high-quality distilled datasets. We start by showing how to establish a strong baseline that already achieves state-of-the-art accuracy through leveraging recent advancements and thoughtful adjustments in model design and optimization processes. By integrating distributions and predictions from a committee of models while generating accurate soft labels, our method captures a wider spectrum of data features, reduces model-specific biases and mitigates distributional shifts between synthetic data and original data. This voting-based strategy not only promotes diversity and robustness within the distilled dataset but also significantly reduces overfitting, resulting in improved performance on post-eval tasks. Extensive experiments across various datasets and IPCs (images per class) demonstrate that Committee Voting leads to more reliable and adaptable distilled data compared to single/multi-model distillation methods, demonstrating its potential for efficient and accurate dataset distillation.

## Keywords
Efficient Learning, Green AI
