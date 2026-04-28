# Precise Attribute Intensity Control in Large Language Models via Targeted Representation Editing

**Venue:** iclr2026 (Desk Reject)
**Authors:** Rongzhi Zhang, Liqin Ye, Yuzhao Heng, Xiang Chen, Tong Yu, Lingkai Kong, Sudheer Chava, Chao Zhang
**OpenReview:** [https://openreview.net/forum?id=364eoDZes9](https://openreview.net/forum?id=364eoDZes9)

## Relevance

**LLM score:** 1/3 — The paper focuses on controlled text generation via representation editing, with efficiency mentioned only as a downstream application, not as a core contribution to energy-efficient training or Sutro Group priorities.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
Precise attribute intensity control—generating Large Language Model (LLM) outputs with specific, user-defined attribute intensities—is crucial for AI systems adaptable to diverse user expectations.
Current LLM alignment methods, however, typically provide only directional or open-ended guidance, failing to reliably achieve exact attribute intensities. 
We address this limitation with three key designs: (1) reformulating precise attribute intensity control as a target-reaching problem, rather than simple maximization; (2) training a lightweight value function via temporal-difference learning to predict final attribute intensity scores from partial generations, thereby steering LLM outputs; and (3) employing gradient-based interventions on hidden representations to navigate the model precisely towards specific attribute intensity targets.
Our method enables fine-grained, continuous control over attribute intensities, moving beyond simple directional alignment.
Experiments on \llama and \PHI confirm our method's ability to steer text generation to user-specified attribute intensities with high accuracy.
Finally, we demonstrate efficiency enhancements across three downstream tasks: preference data synthesis, Pareto frontier approximation and optimization, and distillation of aligned behaviors for intervention-free inference. Our code is available on \href{https://anonymous.4open.science/r/pre-control-F482}{https://anonymous.4open.science/r/pre-control-F482}.

## Keywords
Preference Control, Representation Editing, Large Language Models
