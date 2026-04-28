# LoRA: The Past, Present, and Future

**Venue:** iclr2026 (Withdraw)
**Authors:** Elijah Cadenhead, Cristian McGee, Xin Li, El houcine Bergou, Aritra Dutta
**OpenReview:** [https://openreview.net/forum?id=0bvYEPH1O5](https://openreview.net/forum?id=0bvYEPH1O5)

## Relevance

**LLM score:** 1/3 — The paper focuses on parameter-efficient fine-tuning (LoRA variants), tangentially relevant as it mentions computational and memory overhead but not directly advancing energy-efficient training, data movement, sparsity, or biologically-plausible learning.
**Keyword hits:** `low-rank, lora`

## TLDR
(none provided)

## Abstract
Full fine-tuning of large pre-trained models is constrained by computational and memory overhead, motivating parameter-efficient fine-tuning approaches, such as low-rank adaptation (LoRA) and its variants. Yet, questions remain about their convergence behavior, comparative generalization, and practical limits compared to full fine-tuning. We present a historical framing (the past: full fine-tuning and original LoRA; the present: different variants of LoRA) and introduce simpler, cheaper, parameter-efficient extensions: Cheap LoRA (cLA)—training a single low-rank factor with the other fixed (deterministically or, in its randomized variant, stochastically)—and the chained circulant variant, ${c}^3$LA. While analyzing these LoRA variants, we realized that nonconvex convergence analysis is only feasible for the variants where one low-rank factor is kept frozen; for LoRA, Lipschitz smoothness of the loss function does not hold. However, we derived information-theoretic generalization error bounds for all variants, which, to our knowledge, is one of the first endeavors in this area. We conduct an extensive empirical study that spans $7$ LoRA-based methods and full fine-tuning across $9$ pre-trained models on diverse tasks and datasets, and dissect their performance using a multitude of analytical tools, including the loss landscape of the resulting fine-tuned models, their spectral properties, and generalizability. Despite the theoretical results, our experimental study shows that fine-tuning performance, in practice, may or may not be better, depending on the actual trained model, the datasets used, and multiple other factors. In summary, the performance of LoRA-based PEFT methods suggests that using their cheaper variants would be advantageous for effective cost reduction and improved generalizability of pre-trained models.

## Keywords
Parameter Efficient Fine Tuning
