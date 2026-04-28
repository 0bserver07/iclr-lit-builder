# Listens like Mel: Boosting Latent Audio Diffusion with Channel Locality

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5PBKxl7o49](https://openreview.net/forum?id=5PBKxl7o49)

## Relevance

**LLM score:** 2/3 — Faster convergence directly improves training efficiency, making efficiency a main contribution, though it does not specifically address data movement, sparse parity, or hardware-aware methods.
**Keyword hits:** `locality`

## TLDR
(none provided)

## Abstract
Latent representations critically shape diffusion-based audio generation. We observe that Mel spectrograms exhibit an approximate power-law spectrum that aligns with diffusion’s coarse-to-fine denoising, whereas waveform variational autoencoder (VAE) latents are nearly equal intensity along the channel axis. We introduce channel-span masking, which in expectation behaves like a rectangular window across channels and thus a low-pass filter in the channel-frequency domain, increasing channel locality. The induced locality steepens latent spectral slopes toward a power-law distribution and leads to up to $2\text{--}4\times$ faster convergence of Diffusion Transformer (DiT) training on audio generation tasks, while maintaining reconstruction fidelity and compression. Experimental results show that the model performs comparably to, or better than, competitive baselines under the same conditions. Our codes are available at https://anonymous.4open.science/r/lafa-F2A2

## Keywords
audio generation, variational auto-encoder, representation learning, self-supervised learning
