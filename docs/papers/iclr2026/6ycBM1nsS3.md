# CoDA: From Text-to-Image Diffusion Models to Training-Free Dataset Distillation

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6ycBM1nsS3](https://openreview.net/forum?id=6ycBM1nsS3)

## Relevance

**LLM score:** 2/3 — The paper's main contribution is a training-free dataset distillation method that eliminates the prohibitive cost of pre-training a generative model on the full dataset, directly addressing training efficiency and aligning with Sutro Group's distillation interest.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
Prevailing Dataset Distillation (DD) methods leveraging generative models confront two fundamental limitations. First, despite pioneering the use of diffusion models in DD and delivering impressive performance, the vast majority of approaches paradoxically require a diffusion model pre-trained on the full target dataset, undermining the very purpose of DD and incurring prohibitive training costs. Second, although some methods turn to general text-to-image models without relying on such target-specific training, they suffer from a significant distributional mismatch, as the web-scale priors encapsulated in these foundation models fail to faithfully capture the target-specific semantics, leading to suboptimal performance. To tackle these challenges, we propose Core Distribution Alignment (CoDA), a framework that enables effective DD using only an off-the-shelf text-to-image model. Our key idea is to first identify the ``intrinsic core distribution'' of the target dataset using a robust density-based discovery mechanism. We then steer the generative process to align the generated samples with this core distribution. By doing so, CoDA effectively bridges the gap between general-purpose generative priors and target semantics, yielding highly representative distilled datasets. Extensive experiments suggest that, without relying on a generative model specifically trained on the target dataset, CoDA achieves performance on par with or even superior to previous methods with such reliance across all benchmarks, including ImageNet-1K and its subsets. Notably, it establishes a new state-of-the-art accuracy of 60.4\% at the 50-images-per-class (IPC) setup on ImageNet-1K. Our code is available on the project webpage: https://github.com/zzzlt422/CoDA

## Keywords
Dataset Distillation, Text-to-Image Diffusion Model, Core Distribution Alignment
