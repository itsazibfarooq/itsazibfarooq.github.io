---
layout: page
title: Diffusion Deblurring with a Motion Prior
description: LoRA fine-tuning of a U-Net diffusion denoiser with a high-frequency loss and a motion prior.
importance: 4
category: research
---

- Improved a U-Net diffusion denoiser's fidelity on fine, small-scale structures by fine-tuning with LoRA under a high-pass reconstruction loss that emphasizes edges.
- Added an object-motion prior from a three-frame history, estimating displacement, velocity, and acceleration to regularize temporal consistency.
