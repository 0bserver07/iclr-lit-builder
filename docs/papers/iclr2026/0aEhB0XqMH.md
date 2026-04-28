# Learning-Domain Decomposition: Interpreting Training Dynamics via Loss Vectors

**Venue:** iclr2026 (Withdraw)
**Authors:** Koshiro Aoki, Masaru Isonuma, Yusuke Oda, Hirokazu Kiyomaru, Takashi Kodama, Chaoran Liu, Yohei Oseki, Yusuke Miyao, Daisuke Kawahara
**OpenReview:** [https://openreview.net/forum?id=0aEhB0XqMH](https://openreview.net/forum?id=0aEhB0XqMH)

## Relevance

**LLM score:** 2/3 — The paper's data pruning method, enabling training with 5% of data, directly contributes to training efficiency and data reduction, aligning with the group's focus on efficient AI training.
**Keyword hits:** `pruning, sparse`

## TLDR
(none provided)

## Abstract
Deep neural networks achieve high performance, but it is still not well understood how they learn during training and when they forget what has been learned. In this study, we propose Learning-Domain Decomposition (LDD), a method that analyzes training dynamics based on per-sample loss vectors. LDD applies sparse dictionary learning to the differences of loss vectors across training steps. This enables the extraction of learning-domains, which represent common patterns learned by the model, and clarifies when they are acquired or forgotten in a bottom-up manner. We further evaluate the contribution of each domain to generalization by quantifying its effect on validation loss. Experiments on the MNIST dataset with a simple CNN show that easy samples are learned early but later degrade generalization, while ambiguous samples are repeatedly forgotten and relearned and ultimately contribute to generalization. In addition, data pruning based on the degree of contribution to multiple domains (domain multiplicity) allows training with 5\% of the data while achieving performance comparable to or better than training with the full dataset. These findings demonstrate that LDD provides both an interpretable perspective on training dynamics and a practical tool for efficient data selection.

## Keywords
Training Dynamics, Loss Vectors, Interpretability, Data Pruning
