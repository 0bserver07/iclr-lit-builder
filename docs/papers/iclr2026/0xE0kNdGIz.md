# Vulcan: Crafting Compact Class-Specific Vision Transformers For Edge Intelligence

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0xE0kNdGIz](https://openreview.net/forum?id=0xE0kNdGIz)

## Relevance

**LLM score:** 1/3 — The paper uses structured pruning for post-training model compression, touching on sparsity but not focusing on training efficiency or other Sutro Group training-related priorities.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Large Vision Transformers (ViTs) must often be compressed before they can be deployed on resource-constrained edge devices. 
However, many edge devices require only part of the *all-classes* knowledge of a pre-trained ViT in their corresponding application scenarios. This is overlooked by existing compression methods. Lightweight models produced by these methods retain a substantial amount of class-irrelevant knowledge and suffer suboptimal performance on target classes. To address this, we analyze the knowledge distribution of ViT and reveal a knowledge disentanglement within it: neurons in the feed-forward network (FFN) modules encode class-specific knowledge, while the multi-head attention (MHA) modules capture class-agnostic patterns. Building on this insight, we introduce Vulcan, a pruning-oriented post-training method for deriving compact class-specific models from a pre-trained ViT under given resource budgets. Vulcan follows a novel *train-then-prune* paradigm, which introduces redundancy into ViTs deliberately by collapsing FFN neurons onto those with the highest class-specific activations and by enforcing low-rankness in MHA weights. This design mitigates the irreversible knowledge loss of direct pruning, so that the post-trained model can be compressed into a compact one with negligible performance loss. Notably, the derived edge ViTs not only achieve significant reductions in size and computation but also even surpass the original ViTs in performance on specific classes. Comprehensive experiments with five base ViTs covering three representative visual tasks on four datasets demonstrate that Vulcan-derived ViTs outperform the base ViTs on class-specific tasks by up to 15.12\% in accuracy, with only 20\%–40\% of their sizes. Compared with state-of-the-art structured pruning methods, Vulcan improves class-specific accuracy by up to 13.92\%. Code is available at [Vulcan](https://github.com/CGCL-codes/Vulcan).

## Keywords
Class-specific model derivation, Vision Transformer, structured pruning, edge intelligence
