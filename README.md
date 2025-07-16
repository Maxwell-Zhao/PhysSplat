# [ICCV2025] Efficient Physics Simulation for 3D Scenes via MLLM-Guided Gaussian Splatting

This is the official code for [PhysSplat](https://arxiv.org/pdf/2411.12789).

## Introduction
Recent advancements in 3D generation models have opened new possibilities for simulating dynamic 3D object movements and customizing behaviors, yet creating this content remains challenging. Current methods often require manual assignment of precise physical properties for simulations or rely on video generation models to predict them, which is computationally intensive. In this paper, we rethink the usage of multi-modal large language model (MLLM) in physics-based simulation, and present PhysSplat, a physics-based approach that efficiently endows static 3D objects with interactive dynamics. We begin with detailed scene reconstruction and object-level 3D open-vocabulary segmentation, progressing to multi-view image in-painting. Inspired by human visual reasoning, we propose MLLMbased Physical Property Perception (MLLM-P3) to predict the mean physical properties of objects in a zero-shot manner. The Material Property Distribution Prediction model (MPDP) then estimates physical property distributions via geometry-conditioned probabilistic sampling of MLLM-P3 outputs, reformulating the problem as probability distribution estimation to reduce computational costs. Finally, we simulate objects in 3D scenes with particles sampled via the Physical-Geometric Adaptive Sampling (PGAS) strategy, efficiently capturing complex deformations and significantly reducing computational costs. Extensive experiments
and user studies demonstrate that our PhysSplat achieves more realistic motion than state-of-the-art methods within 2 minutes on a single GPU.

## Installation





