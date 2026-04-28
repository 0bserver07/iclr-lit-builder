# Diversity of Transformer Layers: One Aspect of Parameter Scaling Laws

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=35KC8ozdIO](https://openreview.net/forum?id=35KC8ozdIO)

## Relevance

**LLM score:** 1/3 — Paper analyzes layer diversity and parameter scaling laws from an interpretability perspective, tangentially relevant to Sutro Group's interest in scaling laws but not directly advancing energy-efficient training.
**Keyword hits:** `scaling law`

## TLDR
(none provided)

## Abstract
Transformers deliver outstanding performance across a wide range of tasks and are now a dominant backbone architecture for large language models (LLMs). Their task-solving performance is improved by increasing parameter size, as shown in the recent studies on the Scaling Law for parameters. Although recent mechanistic-interpretability studies have deepened our understanding of internal behavior by analyzing the residual stream, the relationship between these internal mechanisms and the Scaling Law for parameters remains unclear. That hinders the efficient performance improvement of Transformers. To bridge this gap, we propose a theoretical framework that formulates the contribution of each layer, composed of modules such as the embedding layer, Multi-head Attention (MHA), and Multi-layer Perceptron (MLP) within the residual stream through a bias–diversity decomposition. The decomposition separates (i) bias, the error of each layer's output from the ground truth, and (ii) diversity, which indicates how much the outputs of each layer differ from each other. Analyzing Transformers under this framework reveals that performance improves when individual layers make predictions close to the correct answer and remain mutually diverse. We show that diversity becomes especially critical when individual layers' outputs are far from the ground truth. Furthermore, we introduce an information-theoretic treatment of bias and diversity and indicate that adding layers enhances performance only when those layers behave differently, i.e., are diverse. Moreover, we also reveal the performance gains from increasing the number of layers exhibit submodularity: marginal improvements diminish as additional layers increase, mirroring the logarithmic convergence predicted by the Scaling Law for parameters. Moreover, experiments on multiple semantic-understanding tasks with various LLMs empirically confirm the theoretical properties derived in this study. Our code will be available at https://github.com/[Anonymous].

## Keywords
Transformer, Residual Stream, Logit Lens, Scaling Law
