# NorMuon: Making Muon more efficient and scalable

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7TeJXgr7L6](https://openreview.net/forum?id=7TeJXgr7L6)

## Relevance

**LLM score:** 3/3 — Directly advances training efficiency and optimizer design, with a distributed implementation that addresses hardware-aware scaling and data movement, aligning with Sutro Group's priorities.
**Keyword hits:** `second-order, optimizer, adam, muon`

## TLDR
(none provided)

## Abstract
The choice of optimizer significantly impacts the training efficiency and computational costs of large language models (LLMs). Recently, the Muon optimizer has demonstrated promising results by orthogonalizing parameter updates, improving optimization geometry through better conditioning.
Despite Muon’s emergence as a candidate successor to Adam, the potential for jointly leveraging their strengths—has not been systematically explored.
In this work, we bridge this gap by proposing NorMuon (Neuron-wise Normalized Muon), an optimizer that synergistically combines orthogonalization with neuron-level adaptive learning rates. Our analysis reveals that while Muon effectively reduces condition numbers, the resulting updates exhibit highly non-uniform neuron norms, causing certain neurons to dominate the optimization process. NorMuon addresses this imbalance by maintaining second-order momentum statistics for each neuron and applying row-wise normalization after orthogonalization, ensuring balanced parameter utilization while preserving Muon's conditioning benefits. To enable practical deployment at scale, we develop an efficient distributed implementation under the FSDP2 framework that strategically distributes orthogonalization computations across devices.
Experiments across multiple model scales demonstrate that NorMuon consistently outperforms both Adam and Muon, achieving 21.74\% better training efficiency than Adam and 11.31\% improvement over Muon on 1.1B pretraining setting, while maintaining a comparable memory footprint to Muon. Our findings suggest that orthogonalization and adaptive learning rates are complementary rather than competing approaches, opening new avenues for optimizer design in large-scale deep learning.

## Keywords
Optimizer, Muon, Training efficiency, large language model
