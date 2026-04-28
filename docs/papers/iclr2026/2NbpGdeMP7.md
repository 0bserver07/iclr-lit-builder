# Boost Post-Training Quantization via Null Space Optimization for Large Language Models

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2NbpGdeMP7](https://openreview.net/forum?id=2NbpGdeMP7)

## Relevance

**LLM score:** 2/3 — The paper focuses on post-training quantization for LLMs, aligning with the Sutro Group's interest in low-precision/quantization techniques.
**Keyword hits:** `quantization`

## TLDR
(none provided)

## Abstract
Existing post-training quantization methods for large language models (LLMs) offer remarkable success. However, the increasingly marginal performance gains suggest that existing quantization strategies are insufficient to support the development of more compressed models. To inspire new directions for future research, this paper introduces the concept of \textbf{null space} into LLMs quantization. We argue that the quantization error can be effectively alleviated by constraining the post-quantization weight perturbation to lie within the null space of input activations. To prove this fresh idea, we propose an intuitive projection method on several PTQ baselines to validate whether the performance will be further improved. Specifically, we devise an efficient and accurate null space projection approximation tailored to the characteristics of LLMs, and then theoretically derive a closed-form solution for an equivalent vector of the obtained projection matrix to satisfy practical inference condition. When validating our method on several milestone PTQ baselines, further performance improvements can be noticed obviously, demonstrating the novel perspective of null space optimization for LLMs quantization is effective. We view this paper the first step to alleviate the quantization error based on the insights of null space, hoping it inspiring future researchers to design more advanced quantization methods. Codes are available at \url{https://anonymous.4open.science/r/q2n-2236}.

## Keywords
Large Language Models, Post-training Quantization, Null space optimization
