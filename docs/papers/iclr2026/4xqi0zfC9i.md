# Trading Complexity for Expressivity: Theoretical Exploration of Linear and Causal Token Mixing Strategies

**Venue:** iclr2026 (Withdraw)
**Authors:** Erwan Fagnou, Paul Caillon, Blaise Delattre, Alexandre Allauzen
**OpenReview:** [https://openreview.net/forum?id=4xqi0zfC9i](https://openreview.net/forum?id=4xqi0zfC9i)

## Relevance

**LLM score:** 1/3 — Mentions decoding speed and cache size as design tradeoffs, but the main contribution is a theoretical framework for token mixing architectures, not directly advancing energy-efficient training or Sutro Group priorities.
**Keyword hits:** `cache`

## TLDR
(none provided)

## Abstract
We revisit token mixing in sequence models through a unified, causal linear framework that separates two effects: (i) direct one-step influence of inputs on outputs and (ii) recurrent propagation of information through past outputs. This perspective encompasses major architectures -- including attention, state-space models, and hybrids -- while exposing simple design parameters that govern efficiency and expressivity. We show that every causal linear mixer can be written in this form, where computation reduces to solving a triangular system with well-understood numerical properties.
    The framework generalizes the recurrence equations of SSMs and linear attention by allowing each state to depend on multiple past states rather than only the immediate predecessor. This unlocks new tradeoffs between decoding speed, cache size, and ability to model long-range dependencies.
    Building on this view, we design structured recurrence patterns that provably achieve any desired complexity -- trading runtime for expressivity in a principled way. Together, these results provide a unified toolkit for understanding and designing efficient, expressive token mixers across model families.

## Keywords
token mixing, linear recurrence
