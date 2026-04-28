# Critique-Guided Distillation for Efficient and Robust Language Model Reasoning

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2EvMmC23sC](https://openreview.net/forum?id=2EvMmC23sC)

## Relevance

**LLM score:** 2/3 — The paper proposes a knowledge distillation method that significantly reduces compute requirements (144x less than RL), directly advancing training efficiency, which aligns with the Sutro Group's focus on distillation and efficient training.
**Keyword hits:** `knowledge distillation, distillation`

## TLDR
(none provided)

## Abstract
Supervised fine-tuning (SFT) with expert demonstrations often suffers from the imitation problem, where models reproduce correct responses without internalizing the underlying reasoning. We propose $\text{C{\small RITIQUE-}G{\small UIDED} D{\small ISTILLATION} (CGD)}$, a multi-stage training framework that augments SFT with teacher-generated $\textit{explanatory critiques}$ and $\textit{refined responses}$. Instead of directly imitating teacher outputs, a student learns to map the triplet of prompt, its own initial response, and teacher critique into the refined teacher response, thereby capturing both $\textit{what}$ to output and $\textit{why}$. On mathematical reasoning benchmarks, $\text{CGD}$ achieves substantial gains across LLaMA and Qwen families: +15.0\% on AMC23 and +12.2\% on MATH-500 over CFT, while avoiding the format drift that plagues critique-based methods. Cross-family validation on Qwen2.5-Math-7B with diverse teachers (Claude Sonnet 3.7 to weaker open-source models) achieves state-of-the-art performance (50.4 avg, +22.6\% over base) with 144× less compute than RL methods. Critically, despite training on data containing no code, $\text{CGD}$ generalizes to out-of-distribution benchmarks:~+4.88\% on HumanEval (code generation), and preserved or improved performance on GPQA, MUSR, TruthfulQA, and BBH, while CFT suffers catastrophic forgetting (-21.3\% on IFEval). These results establish $\text{CGD}$ as a cost-effective intermediate training paradigm that can serve as a warm-start before reasoning SFT or RL, offering a scalable enhancement to modern LLM training workflows.

## Keywords
Large Language Models, Knowledge Distillation, Critique, Iterative Refinement, Reasoning
