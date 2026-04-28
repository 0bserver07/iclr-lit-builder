# DLM-One: Diffusion Language Models for One-Step Sequence Generation

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4g3dTrLnoF](https://openreview.net/forum?id=4g3dTrLnoF)

## Relevance

**LLM score:** 1/3 — The paper uses score distillation to achieve efficient one-step inference, which tangentially relates to the group's interest in distillation, but its main focus is on sampling speed, not energy-efficient training or hardware-aware techniques.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
This paper introduces *DLM-One*, a score-distillation-based framework for one-step sequence generation with continuous diffusion language models (DLMs). DLM-One eliminates the need for iterative refinement by aligning the scores of a student model’s outputs in the continuous token embedding space with the score function of a pretrained teacher DLM. We investigate whether DLM-One can achieve substantial gains in sampling efficiency for language modeling. Through comprehensive experiments on DiffuSeq—a representative continuous DLM—we show that DLM-One achieves up to $\mathord{\sim}500\times$ speedup in inference time while maintaining competitive performance on benchmark text generation tasks used to evaluate the teacher models. We further analyze the method’s empirical behavior across multiple datasets, providing initial insights into its generality and practical applicability. Our findings position one-step diffusion as a promising direction for efficient, high-quality language generation and broader adoption of continuous diffusion models operating in embedding space for natural language processing.

## Keywords
Generative Modeling, Score Distillation, Non-autoregressive
