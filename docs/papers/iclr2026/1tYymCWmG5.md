# DeFake: Data-Efficient Adaptation for Generalized Deepfake Detection

**Venue:** iclr2026 (Withdraw)
**Authors:** Debarshi Brahma, Suvam Dey, Anuska Roy, Soma Biswas
**OpenReview:** [https://openreview.net/forum?id=1tYymCWmG5](https://openreview.net/forum?id=1tYymCWmG5)

## Relevance

**LLM score:** 1/3 — The paper focuses on data-efficient adaptation (few-shot learning for deepfake detection), which is tangential to the energy-efficiency and hardware-aware training priorities of the Sutro Group.
**Keyword hits:** `data-efficient`

## TLDR
(none provided)

## Abstract
While deepfake detection methods have seen significant progress, current approaches
focus on detecting fully synthetic or partially manipulated images separately,
and often rely on large amounts of labeled training data. However, in
real world, deepfakes can originate from any paradigm. In this work, we propose
a generalized deepfake detection method, DeFake (Data-Efficient Adaptation for
Generalized Deepfake Detection) which can detect both fully synthetic and partially
manipulated images simultaneously. We reframe the generalization problem
as a data-efficient adaptation of a base synthetic image detector to the task of partial
manipulation detection using limited training samples, without degrading the
original synthetic image detection task. We introduce three novel modules: (a)
Noise-aware Patch Enhancement (NPE) which captures local manipulation artifacts
present in partially manipulated images, (b) Adaptive Score Aggregation
(ASA) which modulates the influence of the global image-level semantics and
the local patch-level artifacts, and (c) Multi-scale alignment which enhances discriminative
learning at both image and patch-level. The proposed modules are
generalizable and can be integrated into various base models. Extensive experiments
on 14 datasets across both paradigms demonstrate the effectiveness of our
proposed DeFake, outperforming state-of-the-art approaches in both settings.

## Keywords
Deepfake detection, Data-efficient learning, Vision-language models
