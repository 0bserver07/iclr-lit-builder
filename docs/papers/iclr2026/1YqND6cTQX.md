# Personalization Under Value Conflict: Resolving Contradictory Preferences with Paired Fine-Tuning

**Venue:** iclr2026 (Withdraw)
**Authors:** Shanyong Wang, Shuhang Lin, Yining Zhao, Xi Zhu, Yongfeng Zhang
**OpenReview:** [https://openreview.net/forum?id=1YqND6cTQX](https://openreview.net/forum?id=1YqND6cTQX)

## Relevance

**LLM score:** 1/3 — The paper mentions reduced data requirements as a secondary benefit, but the main contribution is personalization under value conflict, not energy-efficient training or Sutro Group's core priorities like data movement, sparsity, or low-precision.
**Keyword hits:** `data-efficient`

## TLDR
(none provided)

## Abstract
Large language models (LLMs) are increasingly expected to capture not only broadly shared human universal values but also the diverse and often contradictory preferences of individual users. Existing alignment approaches typically optimize for a single preference direction, making them unsuitable when users switch between opposing values. We propose \textbf{Preference-Paired Fine-Tuning (PFT)}, a framework that trains models on paired contradictory preferences, enabling a single model to align with both sides simultaneously. Beyond handling one preference pair, PFT generalizes to multiple mutually exclusive preference dimensions, capturing shared structures across conflicts. With only a few in-context examples from user history, PFT further enables rapid and data-efficient customization, yielding stronger alignment to individual preferences. Experiments show that PFT achieves up to $\textbf{96.7\% }$classification accuracy, improves open-ended generation scores by $\textbf{up to 20.05\%}$, and reduces data requirements by about $\textbf{40\%}$ compared to single-preference fine-tuning. These results highlight a scalable path toward conflict-aware and personalized LLMs.

## Keywords
Preference confict, Personalization
