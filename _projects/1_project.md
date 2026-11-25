---
layout: page
title: Large-Scale Synthetic Data Generation
description: A 10 TB multi-view driving dataset generated on a 20xV100 cluster with CARLA.
importance: 1
category: research
---

- Generated a 10 TB multi-view driving dataset in under two weeks on a modest 20xV100 multi-node cluster through an optimized parallel generation pipeline.
- Built the pipeline on the CARLA simulator (Unreal Engine 4), producing synchronized multi-view video with per-frame camera parameters and driving-infraction annotations.
- Diagnosed and fixed a memory leak in CARLA that had prevented stable parallelization.
- Made the pipeline fault-tolerant and fully resumable: worker-level failover isolates a failed seed, and seed-level checkpointing lets a run resume exactly where it stopped.
- Deterministic seeding makes every sample, and the dataset as a whole, exactly regenerable.
- The dataset supports post-training experiments for autonomous driving world models.
