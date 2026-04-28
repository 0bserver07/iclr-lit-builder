# Textual Steering Vectors Can Improve Visual Understanding in Multimodal Large Language Models

**Venue:** iclr2026 (Withdraw)
**Authors:** Haosheng Gan, Deqing Fu, Julian Asilis, Ollie Liu, Vatsal Sharan, Robin Jia, Willie Neiswanger
**OpenReview:** [https://openreview.net/forum?id=3e4vWE1kh8](https://openreview.net/forum?id=3e4vWE1kh8)

## Relevance

**LLM score:** 1/3 — The paper mentions minimal computational overhead but focuses on interpretability and steering for multimodal models, not energy-efficient training or the group's core priorities.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
Steering methods have emerged as effective tools for guiding large language models’ behavior, yet multimodal large language models (MLLMs) lack comparable techniques due to recency and architectural diversity. Inspired by this gap, we demonstrate that steering vectors derived solely from text-only LLM backbones can effectively guide their multimodal counterparts, revealing a novel cross-modal transfer that enables reuse of existing interpretability tools. Using community-standard methods—Sparse Autoencoders (SAE), Mean Shift, and Linear Probing—we systematically validate this transfer effect across diverse MLLM architectures and visual reasoning tasks. Text-derived steering consistently enhances multimodal performance, with mean shift achieving up to +7.3% improvement in spatial relationship accuracy and +3.3% in counting accuracy on CV-Bench, and exhibits strong generalization to out-of-distribution datasets. These results highlight textual steering vectors as a powerful, efficient mechanism for enhancing grounding in MLLMs with minimal additional data collection and computational overhead.

## Keywords
steering vectors, multimodal large language models, interpretability
