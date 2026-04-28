# Cognitive Alignment in Personality Reasoning: Leveraging Prototype Theory for MBTI Inference

**Venue:** iclr2026 (Desk Reject)
**Authors:** Haoyuan Li, YUANBO TONG, Yuchen Li, Zirui Wang, Chunhou Liu, Jiamou Liu
**OpenReview:** [https://openreview.net/forum?id=4HenLycCQ3](https://openreview.net/forum?id=4HenLycCQ3)

## Relevance

**LLM score:** 1/3 — Uses LoRA for parameter-efficient fine-tuning, but the main contribution is cognitively aligned inference, not energy-efficient training or the Sutro Group's core priorities.
**Keyword hits:** `lora`

## TLDR
(none provided)

## Abstract
Personality recognition from text is typically cast as hard-label classification, which obscures the graded, prototype-like nature of human personality judgments. We present \textsc{ProtoMBTI}, a cognitively aligned framework for MBTI inference that operationalizes prototype theory within an LLM-based pipeline. First, we construct a balanced, quality-controlled corpus via LLM-guided multi-dimensional augmentation (semantic, linguistic, sentiment). Next, we LoRA-fine-tune a lightweight ($\leq$2B) encoder to learn discriminative embeddings and to standardize a bank of ``personality prototypes''. At inference, we retrieve top-$k$ prototypes for a query post and perform a retrieve–reuse–revise–retain cycle: the model aggregates prototype evidence via prompt-based voting, revises when inconsistencies arise, and, upon correct prediction, retains the sample to continually enrich the prototype library. Across Kaggle and Pandora benchmarks, \textsc{ProtoMBTI} improves over baselines on both the four MBTI dichotomies and the full 16-type task, and exhibits robust cross-dataset generalization. Our results indicate that aligning the inference process with psychological prototype reasoning yields gains in accuracy, interpretability, and transfer for text-based personality modeling.

## Keywords
Prototype Theory, Cognitive Alignment, MBTI Inference, Interpretability
