---
layout: project
title: PlaNet-ClothPick
subtitle: Effective Fabric Flattening Based on Latent Dynamic Planning
venue: IEEE/SICE SII 2024
authors: Halid Abdulrahim Kadi and Kasim Terzić
affiliation: University of St Andrews
links:
  - { label: Paper, url: "https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10417545" }
  - { label: arXiv, url: "https://arxiv.org/abs/2303.01345" }
  - { label: Benchmarks and Oracles, url: "https://github.com/halid1020/softgym-deepcloth" }
  - { label: Method & Dataset, url: "https://github.com/halid1020/agent-arena-v0/blob/main/projects/planet-clothpick.md" }
abstract: >-
  Why do Recurrent State Space Models such as PlaNet fail at cloth manipulation tasks? Recent work has attributed this to the blurry prediction of the observation, which makes it difficult to plan directly in the latent space. This paper explores the reasons behind this by applying PlaNet in the pick-and-place fabric-flattening domain. We find that the sharp discontinuity of the transition function on the contour of the fabric makes it difficult to learn an accurate latent dynamic model, causing the MPC planner to produce pick actions slightly outside of the article. By limiting picking space on the cloth mask and training on specially engineered trajectories, our mesh-free PlaNet-ClothPick surpasses visual planning and policy learning methods on principal metrics in simulation, achieving similar performance as state-of-the-art mesh-based planning approaches. Notably, our model exhibits a faster action inference and requires fewer transitional model parameters than the state-of-the-art robotic systems in this domain.
sections:
  - title: Method
    groups:
      - cols: 2
        items:
          - { src: 01.png }
          - { src: 02.png }
  - title: Pick-and-Place Fabric Flattening in SoftGym
    groups:
      - title: (a) ClothMaskPick-MPC and MPC-CEM on PlaNet-ClothPick
        cols: 3
        items:
          - { src: 03.mp4, caption: ClothMaskPick-MPC }
          - { src: 04.mp4, caption: MPC-CEM }
          - { src: 05.mp4, caption: Oracle Expert (for reference) }
      - title: (b) Policy Learning Baselines
        cols: 3
        items:
          - { src: 06.mp4, caption: DrQ-SAC }
          - { src: 07.mp4, caption: Curl-SAC }
          - { src: 08.mp4, caption: "Dreamer: Normal" }
          - { src: 09.mp4, caption: "Dreamer: Categorical" }
          - { src: 10.mp4, caption: SLAC }
      - title: (c) Planning Baselines with ClothMaskPick-MPC
        cols: 3
        items:
          - { src: 11.mp4, caption: PlaNet }
          - { src: 12.mp4, caption: "Dreamer: Normal" }
          - { src: 13.mp4, caption: "Dreamer: Categorical" }
          - { src: 14.mp4, caption: SLAC }
bibtex: |
  @inproceedings{kadi2024planet,
    title={PlaNet-ClothPick: effective fabric flattening based on latent dynamic planning},
    author={Kadi, Halid Abdulrahim and Terzi{\'c}, Kasim},
    booktitle={2024 IEEE/SICE International Symposium on System Integration (SII)},
    pages={972--979},
    year={2024},
    organization={IEEE}
  }
---
