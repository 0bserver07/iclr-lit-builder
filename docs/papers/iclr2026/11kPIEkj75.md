# Semantic Uncertainty Quantification of Hallucinations in LLMs: A Quantum Tensor Network Based Method

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=11kPIEkj75](https://openreview.net/forum?id=11kPIEkj75)

## Relevance

**LLM score:** 1/3 — The paper touches on efficiency by evaluating robustness under quantization for resource-constrained deployments, but its core contribution is uncertainty quantification for hallucination detection, not energy-efficient training.
**Keyword hits:** `quantization`

## TLDR
(none provided)

## Abstract
Large language models (LLMs) exhibit strong generative capabilities but remain vulnerable to confabulations, fluent yet unreliable outputs that vary arbitrarily even under identical prompts. Leveraging a quantum tensor network–based pipeline, we propose a quantum physics-inspired uncertainty quantification framework that accounts for the aleatoric uncertainty in token sequence probability for semantic equivalence-based clustering of LLM generations. In turn, this offers a principled and interpretable scheme for hallucination detection. We further introduce an entropy-maximization strategy that prioritizes high-certainty, semantically coherent outputs and highlights entropy regions where LLM decisions are likely to be unreliable, offering practical guidelines for when human oversight is warranted. We evaluate the robustness of our scheme under different generation lengths and quantization levels, dimensions overlooked in prior studies, demonstrating that our approach remains reliable even in resource-constrained deployments. A total of 116 experiments on TriviaQA, NQ, SVAMP, and SQuAD across multiple architectures (Mistral-7B, Mistral-7B-instruct, Falcon-rw-1b, LLaMA-3.2-1b, LLaMA-2-13b-chat, LLaMA-2-7b-chat, LLaMA-2-13b and LLaMA-2-7b) show consistent improvements in AUROC and AURAC over state-of-the-art baselines.

## Keywords
Semantic uncertainty, Large language models, quantum physics
