# Learning What Matters: Prioritized Concept Learning via Relative Error-driven Sample Selection

**Venue:** iclr2026 (Withdraw)
**Authors:** Qian Yang, Shivam Chandhok, Oscar Mañas, Kanishk Jain, Aishwarya Agrawal, Leonid Sigal
**OpenReview:** [https://openreview.net/forum?id=6xRTMnSQ4K](https://openreview.net/forum?id=6xRTMnSQ4K)

## Relevance

**LLM score:** 1/3 — The paper proposes a sample selection curriculum to improve data and compute efficiency, which is tangentially related to training efficiency but does not directly address Sutro Group's core themes like data movement, sparsity, quantization, or hardware-aware methods.
**Keyword hits:** `compute-efficient`

## TLDR
(none provided)

## Abstract
Instruction tuning has been central to the success of recent vision-language models (VLMs), but it remains expensive—requiring large scale datasets, high-quality annotations and large-compute budget. We propose $\textbf{PR}$ioritized c$\textbf{O}$ncept learnin$\textbf{G}$ via $\textbf{R}$elative $\textbf{E}$rror-driven $\textbf{S}$ample $\textbf{S}$election -- $\textbf{PROGRESS}$ -- a data- and compute-efficient framework that enables VLMs to dynamically select what to learn next based on their evolving needs during training. At each stage, the model tracks its learning progress across skills and selects the most informative samples: those it has not already mastered and are not too difficult to learn at the current state of training. This strategy effectively controls skill acquisition and the order in which skills are learned. Specifically, we sample from skills showing the highest learning progress, prioritizing those with the most rapid improvement. Unlike prior methods, PROGRESS requires no upfront answer annotations, querying answers only on a need basis, avoids reliance on additional supervision from auxiliary VLM, or compute-heavy gradient computations for data selection. Experiments across multiple instruction-tuning datasets of varying scales demonstrate that PROGRESS consistently outperforms state-of-the-art baselines with much less data and supervision. Additionally, we show strong cross-architecture generalization to different VLMs and transferability to larger models, validating PROGRESS as a scalable solution for efficient learning.

## Keywords
Efficient Learning, VLMs, Curriculum Learning
