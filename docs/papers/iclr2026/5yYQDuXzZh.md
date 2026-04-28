# DTP: A Simple yet Effective Distracting Token Pruning Framework for Vision-Language Action Models

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5yYQDuXzZh](https://openreview.net/forum?id=5yYQDuXzZh)

## Relevance

**LLM score:** 1/3 — The paper proposes token pruning (a form of sparsity) but focuses on inference-time performance improvement rather than energy-efficient training or data movement, making it only tangentially related to Sutro Group's training-centric priorities.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Vision-Language Action (VLA) models have shown remarkable progress in robotic manipulation by leveraging the powerful perception abilities of Vision-Language Models (VLMs) to understand environments and directly output actions. However, by default, VLA models may overly attend to image tokens in the task-irrelevant region, which we describe as ‘distracting tokens’. This behavior can disturb the model from the generation of the desired action tokens in each step, affecting the success rate of tasks. In this paper, we introduce a simple yet effective plug-and-play Distracting Token Pruning (DTP) framework, which dynamically detects and prunes these distracting image tokens. By correcting the model’s visual attention patterns, we aim to improve the task success rate, as well as exploring the performance upper boundaries of the model without altering its original architecture or adding additional inputs. Experiments on the SIMPLER Benchmark (Li et al., 2024) show that our method consistently achieving relative improvements in task success rates across different types of novel VLA models, demonstrating generalizability to transformer-based VLAs. Further analysis reveals a negative correlation between the task success rate and the amount of attentions in the task-irrelevant region for all models tested, highlighting a common phenomenon of VLA models that could guide future research. We also publish our code at: https://anonymous.4open.science/r/CBD3.

## Keywords
Token Pruning, Visual Attention Pattern, Vision-Language Action, Vision-Language Models
