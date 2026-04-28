# TASTE: Text-Aligned Speech Tokenization and Embedding for Spoken Language Modeling

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6STb8DauN1](https://openreview.net/forum?id=6STb8DauN1)

## Relevance

**LLM score:** 1/3 — The paper uses LoRA for parameter-efficient fine-tuning and reduces sequence length via tokenization, touching efficiency tangentially, but the main contribution is speech-text alignment for spoken language modeling, not training efficiency or Sutro Group's core priorities.
**Keyword hits:** `low-rank`

## TLDR
(none provided)

## Abstract
Recent efforts target spoken language models (SLMs) that not only listen but also speak for more natural human-LLM interaction. Joint text-speech modeling is a promising direction to achieve this. However, the effectiveness of recent speech tokens for joint modeling remains under-explored. To address this, we introduce Text-Aligned Speech Tokenization and Embedding (TASTE), a method that directly addresses the modality gap by aligning speech token with the corresponding text transcription during the tokenization stage. We propose a method that can achieve this through a attention-based aggregation mechanism and with speech reconstruction as the training objective. We have conducted extensive experiments to demonstrate that TASTE can preserve essential paralinguistic information while dramatically reducing the token sequence length. Moreover, TASTE enables straightforward joint spoken language modeling by using Low-Rank Adaptation on the pre-trained text LLM. Our experimental results show that joint modeling with TASTE outperforms other pre-trained SLMs in tasks such as speech continuation and likelihood-based next-speech selection, showcasing its effectiveness. To our best knowledge, TASTE is the first end-to-end approach that utilizes a reconstruction objective to learn a joint tokenization and embedding tailored for text-speech spoken language modeling.

## Keywords
spoken language modeling, speech tokenization
