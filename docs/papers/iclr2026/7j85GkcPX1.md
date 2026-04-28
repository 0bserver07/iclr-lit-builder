# MEDSPIKEFORMER: All Neurons Matter for Medical Image Segmentation

**Venue:** iclr2026 (Withdraw)
**Authors:** Yongquan Xue, Marcin Pietron, Roberto Corizzo, Zhaoru Guo, Chunlei Xu, Yahong Han, Liejun Wang, Panpan Zheng
**OpenReview:** [https://openreview.net/forum?id=7j85GkcPX1](https://openreview.net/forum?id=7j85GkcPX1)

## Relevance

**LLM score:** 1/3 — Tangentially mentions energy efficiency of spiking neural networks, but the main contribution is improving medical image segmentation accuracy through a new attention mechanism and distribution alignment loss, not advancing energy-efficient training or the Sutro Group's specific priorities.
**Keyword hits:** `energy-efficient`

## TLDR
(none provided)

## Abstract
Spiking self-attention (SSA) has emerged as a promising approach for medical image segmentation due to its event-driven and energy-efficient nature. However, segmentation performance still degrades in complex scenarios where salient and non-salient regions coexist. Two fundamental issues remain: i) existing SSA mechanisms rely only on activated neurons, overlooking the contextual cues carried by inactivated neurons, and ii) the binary spike representation causes distribution distortions that make spiking self-attention lag behind their ANN-based self-attention (SA) in spatial discriminability. To overcome these challenges, we propose MedSpikeFormer, a spiking transformer built on the principle that all neurons matter, both activated and inactivated. MedSpikeFormer introduces a Spike-based Decomposed Self-Attention (SDSA) that explicitly models four types of neuronal interactions: activated–activated, activated–inactivated, inactivated–activated, and inactivated–inactivated, thus recovering rich contextual dependencies ignored by conventional SSA. Furthermore, we employ a distribution alignment loss that minimizes the divergence between SDSA and ANN-based self-attention (SA), significantly closing the performance gap to improve spatial feature discriminability while maintaining the binary nature of spiking neural networks. Extensive experiments on five medical segmentation benchmarks demonstrate that MedSpikeFormer consistently outperforms 14 state-of-the-art
methods, achieving up to +2.4% mIoU on ISIC2018 and +8.7% on COVID-19. These results confirm that leveraging both fired and non-fired neurons is crucial for robust spike-driven medical image segmentation. Code is available at https://github.com/AnonymousPaper2026/MedSpikeFormer.

## Keywords
Medical image segmentation, Spiking self-attention, Self-attention, Spike neural network
