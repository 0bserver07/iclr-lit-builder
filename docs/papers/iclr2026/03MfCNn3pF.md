# PersonalQ: Select, Quantize, and Serve Personalized Diffusion Models for Efficient Inference

**Venue:** iclr2026 (Withdraw)
**Authors:** Qirui Wang, Qi Guo, Shanmin Pang, Ming-Ming Cheng, Qing Guo
**OpenReview:** [https://openreview.net/forum?id=03MfCNn3pF](https://openreview.net/forum?id=03MfCNn3pF)

## Relevance

**LLM score:** 1/3 — The paper focuses on inference-time quantization for personalized diffusion models, tangentially related to low-precision but not to energy-efficient training or other Sutro Group training priorities.
**Keyword hits:** `quantization`

## TLDR
(none provided)

## Abstract
Personalized text-to-image generation enables users to create custom AI models that generate their unique concepts—specific objects or artistic styles—achieving unprecedented creative control. However, deploying a large repository of personalized checkpoints faces two critical challenges: (1) ambiguous user prompts make it difficult to match the intended checkpoint in large repositories, and (2) standard post-training quantization methods degrade personalized diffusion checkpoints’ image quality. We analyze the importance of reasoning over checkpoint metadata and clarifying user prompts for intent-aligned checkpoint selection. Additionally, we find that trigger tokens for personalized diffusion play a crucial role in quantization. To address the challenges, we propose PersonalQ, a unified system with two components: Check-in analyzes checkpoint repositories and clarifies user intent for intent-aligned selection, and TAQ (Trigger-Aware Quantization), which protects the trigger-token-related representation to deliver high-quality inference from the chosen checkpoint under quantization. On our Repo-Prompts benchmark, PersonalQ achieves an 89% checkpoint-selection preference win rate and a 4.42/5 intent score. Across benchmarks, TAQ reduces inference memory by up to 75% while maintaining strong text-image alignment (CLIP score 0.297 vs. 0.315 at full precision) and image fidelity (FID 11.03 at W8A8 vs. 10.96 at full precision), enabling scalable deployment of personalized models without compromising quality.

## Keywords
Personalized text-to-image generation
