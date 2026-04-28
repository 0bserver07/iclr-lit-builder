# TreeSNNs: Temporal Resolution Ensembled SNNs for Neuromorphic Action Recognition

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2D0PFUA2lM](https://openreview.net/forum?id=2D0PFUA2lM)

## Relevance

**LLM score:** 1/3 — Mentions SNN energy efficiency as motivation but the main contribution is accuracy improvement via temporal ensembling, not advancing training efficiency, data movement, sparsity, or other Sutro Group priorities.
**Keyword hits:** `energy-efficient, sparse`

## TLDR
(none provided)

## Abstract
Spiking Neural Networks (SNNs) are energy-efficient due to sparse and asynchronous event processing, but their accuracy often lags behind that of conventional ANN deep learning models. Prior research has largely focused on novel SNN architectures and training methods, with continuous event streams typically binned into frames using either fixed event counts or fixed time intervals. In this paper, we observe that different motions exhibit distinct temporal dynamics and may be best captured at different temporal/event resolutions. Building on this insight, we propose TreeSNNs, an ensemble framework where model diversity is expressed via multiple event temporal resolutions. We utilize the Fano factor as a metric to quantify temporal dynamics and guide the selection of such a diverse set of temporal resolutions tailored to a given dataset. Individual SNNs trained at these resolutions are then aggregated through ensembling to improve recognition accuracy. Experiments on three neuromorphic action datasets—DVS Gesture, SL-Animals DVS, and the challenging THU$^{E\text{-}ACT}$-50 CHL—show that TreeSNNs consistently outperform baselines, improving accuracy by 1.05\%–6.8\%.

## Keywords
Spiking Neural Networks, Temporal Ensembling, Neuromorphic Action Recognition
