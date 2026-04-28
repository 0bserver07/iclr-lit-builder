# DomED: Redesigning Ensemble Distillation for Domain Generalization

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6QMQGi9iw9](https://openreview.net/forum?id=6QMQGi9iw9)

## Relevance

**LLM score:** 1/3 — Mentions computational cost reduction via tailored data allocation but main contribution is domain generalization and uncertainty distillation, not core to energy-efficient training priorities.
**Keyword hits:** `knowledge distillation, distillation`

## TLDR
(none provided)

## Abstract
Domain generalization aims to improve model performance on unseen, out-of-distribution (OOD) domains, yet existing methods often overlook the crucial aspect of uncertainty quantification in their predictions. While ensemble learning combined with knowledge distillation offers a promising avenue for enhancing both model accuracy and uncertainty estimation without incurring significant computational overhead at inference time, this approach remains largely unexplored in the context of domain generalization. In this work, we systematically investigate different ensemble and distillation strategies for domain generalization tasks and design a tailored data allocation scheme to enhance OOD generalization as well as reduce computational cost. Our approach trains base models on distinct subsets of domains and performs distillation on complementary subsets, thereby fostering model diversity and training efficiency. Furthermore, we develop a novel technique that decouples uncertainty distillation from the standard distillation process, enabling the accurate distillation of uncertainty estimation capabilities without compromising model accuracy. Our proposed method, $\textit{Domain-aware Ensemble Distillation}$ (DomED), is extensively evaluated against state-of-the-art domain generalization and ensemble distillation techniques across multiple benchmarks, achieving competitive accuracies and substantially improved uncertainty estimates.

## Keywords
Domain generalization, Ensemble learning, Knowledge distillation, Uncertainty quantification
