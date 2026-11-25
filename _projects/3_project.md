---
layout: page
title: Instruction-Guided 3D Scene Editing
description: Text-driven editing of NeRF and 3D Gaussian Splatting scenes.
importance: 3
category: research
---

- Built an editing pipeline for scenes represented as Neural Radiance Fields and 3D Gaussian Splatting, propagating text-driven edits into the 3D representation by iteratively updating the training views.
- Supported both local and global edits by combining the Segment Anything Model (SAM) for region masks with InstructPix2Pix for text-conditioned image editing.
