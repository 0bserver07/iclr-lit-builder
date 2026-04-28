# IOMM: Fast Pre-training of Unified Multimodal Models without Text-Image Pairs

**Venue:** iclr2026 (Withdraw)
**Authors:** Peng Sun, Jun Xie, Tao Lin
**OpenReview:** [https://openreview.net/forum?id=6TkRJ1HgSd](https://openreview.net/forum?id=6TkRJ1HgSd)

## Relevance

**LLM score:** 1/3 — The paper mentions training efficiency (fast pre-training, reduced GPU hours) but its main contribution is data efficiency by using image-only data instead of scarce text-image pairs, not directly advancing the Sutro Group's specific technical priorities like data movement, sparsity, quantization, or local learning.
**Keyword hits:** `data-efficient`

## TLDR
(none provided)

## Abstract
Unified Multimodal Models (UMMs), which integrate deep visual understanding with generative capabilities, are often constrained by inefficient training paradigms and a heavy reliance on scarce, high-quality text-image paired data. In this paper, we systematically analyze existing pre-training recipes for UMMs and identify these two issues as major bottlenecks. To address them, we propose $\textbf{Image-Only Training for UMMs (IOMM)}$, a data-efficient two-stage training framework.
    The first stage pre-trains the visual generative component using abundant unlabeled image-only data, thereby removing the dependency on paired data. The second stage fine-tunes the model using a mixture of unlabeled images and a small curated set of text-image pairs, leading to improved instruction alignment and generative quality.
    Extensive experiments show that IOMM not only improves training efficiency but also achieves state-of-the-art performance.
    For example, our base model IOMM-B, trained generation module from scratch purely on open-source data using approximately only $\textbf{1050}$ H800 GPU hours (including $\textbf{1000}$ hours for image-only pre-training), attains a score of $\textbf{0.89}$ on the GenEval benchmark$\textemdash$surpassing strong baselines such as BAGEL (0.88) and BLIP3-o (0.84).
    Code will be released publicly.

## Keywords
Unified Multimodal model, generative model
