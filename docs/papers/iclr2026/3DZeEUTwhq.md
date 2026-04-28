# Are You Getting What You Pay For? Auditing Model Substitution in LLM APIs

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3DZeEUTwhq](https://openreview.net/forum?id=3DZeEUTwhq)

## Relevance

**LLM score:** 1/3 — Mentions quantization as a potential model substitution but the primary focus is on API integrity auditing, not on advancing training efficiency or related techniques.
**Keyword hits:** `quantized`

## TLDR
(none provided)

## Abstract
Commercial Large Language Model (LLM) APIs create a fundamental trust problem: users pay for specific models but have no guarantee that providers deliver them faithfully. Providers may covertly substitute cheaper alternatives (e.g., quantized versions, smaller models) to reduce costs while maintaining advertised pricing. We formalize this model substitution problem and systematically evaluate detection methods under realistic adversarial conditions. Our empirical analysis reveals that software-only methods are fundamentally unreliable: statistical tests on text outputs are query-intensive and fail against subtle substitutions, while methods using log probabilities are defeated by inherent inference nondeterminism in production environments. We argue that this verification gap can be more effectively closed with hardware-level security. We propose and evaluate the use of Trusted Execution Environments (TEEs) as one practical and robust solution. Our findings demonstrate that TEEs can provide provable cryptographic guarantees of model integrity with only a modest performance overhead, offering a clear and actionable path to ensure users get what they pay for.

## Keywords
API auditing, model substitution
