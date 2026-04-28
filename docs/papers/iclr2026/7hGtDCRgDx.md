# Prompt, Predict, Correct: LLM-TrajEcho for Closed-Loop Trajectory Forecasting via Online Prompt Feedback

**Venue:** iclr2026 (Withdraw)
**Authors:** Yizhou Huang, Yihua Cheng, Kezhi Wang
**OpenReview:** [https://openreview.net/forum?id=7hGtDCRgDx](https://openreview.net/forum?id=7hGtDCRgDx)

## Relevance

**LLM score:** 1/3 — The paper uses LoRA for parameter-efficient fine-tuning, which marginally relates to training efficiency, but its main contribution is closed-loop trajectory forecasting with LLMs, not advancing energy-efficient training or the Sutro Group's core priorities.
**Keyword hits:** `lora`

## TLDR
(none provided)

## Abstract
Accurate trajectory prediction is fundamental to the safety of autonomous vehicles. However, state-of-the-art methods often rely on computationally intensive multi-sensor fusion to achieve high precision, which increases system complexity and hinders real-time deployment. Furthermore, most predictors operate in an open-loop manner, suffering from uncorrected error accumulation. In response, we propose LLM-TrajEcho, a lightweight, end-to-end vision-based framework that eliminates the need for sensor fusion while enabling real-time performance and closed-loop correction. Our framework efficiently encodes spatiotemporal features from video sequences and translates them into structured natural language prompts for a large language model (LLM), leveraging Parameter-Efficient Fine-Tuning (LoRA) to ensure computational efficiency. A key innovation is our online closed-loop feedback mechanism, which dynamically refines the LLM's context based on prediction errors, mitigating long-term drift. Experiments on nuScenes and KITTI Tracking datasets demonstrate that LLM-TrajEcho runs at 0.53 ms per sample, achieves competitive ADE, significantly improves FDE by 30\%, and MR by 21\%. Our work shows that vision-based prediction, combined with LLM reasoning and closed-loop learning, offers a viable path toward accurate and efficient autonomous driving. Demo: https://anonymous.4open.science/r/ICLR-Demo-175B/

## Keywords
Autonomous Driving, Large Language Models, Prompt-based Sequence Modeling, Closed-loop Feedback Learning
