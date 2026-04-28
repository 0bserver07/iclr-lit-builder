# Look Back to Move Forward: Delay-Aware Instance Selection for Online Continual Learning

**Venue:** iclr2026 (Withdraw)
**Authors:** Brenno de Mello Alencar, Heitor Murilo Gomes, Guilherme Weigert Cassales, Bernhard Pfahringer, Albert Bifet, Izak Gama, RICARDO RIOS
**OpenReview:** [https://openreview.net/forum?id=3f1s6yunAJ](https://openreview.net/forum?id=3f1s6yunAJ)

## Relevance

**LLM score:** 1/3 — The paper reduces training budget via selective instance replay, a form of training efficiency, but does not address core Sutro Group priorities like data movement, sparsity, low-precision, or hardware-aware training.
**Keyword hits:** `efficient training`

## TLDR
(none provided)

## Abstract
Supervised continual learning (CL) typically assumes that labels are available immediately after each input arrives. This is unrealistic in many streaming applications, where annotation latency is the norm. When labels arrive late, supervision for past tasks can spill into later tasks, entangling training signals and degrading current performance. We study this delayed-label setting and analyze how different delay regimes impact online CL. We then introduce a delay-aware instance selection strategy that prioritizes which late-labeled examples to use for updates based on a simple, model-utility criterion. By selecting only the most beneficial delayed instances, our approach accelerates performance recovery after task shifts and reduces the training budget when labels from multiple past tasks arrive simultaneously. Our contributions are: (i) a clear problem formulation and evaluation protocol for online continual learning with delayed labels; (ii) an empirical analysis across delay regimes showing how label latency mixes supervision across tasks; and (iii) a plug-and-play instance-selection method compatible with replay-based CL. Experiments indicate consistent improvements in current-task accuracy and stability, with fewer update steps than delay-agnostic baselines.

## Keywords
Online continual learning, delayed labels, Efficient Training, Data Streams
