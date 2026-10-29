---
layout: project
title: LaGarNet
subtitle: Goal-Conditioned Recurrent State-Space Models for Pick-and-Place Garment Flattening
venue: arXiv preprint 2025
authors: Halid Abdulrahim Kadi and Kasim Terzić
affiliation: University of St Andrews
links:
  - { label: arXiv, url: "https://arxiv.org/abs/2508.17070" }
  - { label: Code, url: "https://github.com/st-cortex-lab/LaGarNet" }
  - { label: Dataset & Models, url: "https://drive.google.com/drive/folders/1XZmaZHlttVr4IizSIaFIwCtVYrEf-SkZ?usp=sharing" }
abstract: >-
  We present a novel goal-conditioned recurrent state space (GC-RSSM) model capable of learning latent dynamics of pick-and-place garment manipulation. Our proposed method LaGarNet matches the state-of-the-art performance of mesh-based methods, marking the first successful application of state-space models on complex garments. LaGarNet trains on a coverage-alignment reward and a dataset collected through a general procedure supported by a random policy and a diffusion policy learned from few human demonstrations; it substantially reduces the inductive biases introduced in the previous similar methods. We demonstrate that a single-policy LaGarNet achieves flattening on four different types of garments in both real-world and simulation settings.
sections:
  - title: Garments and Setup
    groups:
      - cols: 2
        items:
          - { src: 01.jpg, caption: Simulated garment types }
          - { src: 04.jpg, caption: Real-world garments and robot setup }
  - title: Real-World Garment Flattening
    groups:
      - cols: 2
        items:
          - { src: 02.mp4 }
          - { src: 03.mp4 }
      - items:
          - { src: 05.jpg }
  - title: Results
    groups:
      - items:
          - { src: 06.png }
          - { src: 07.png }
bibtex: |
  @article{kadi2025lagarnet,
    title={LaGarNet: Goal-Conditioned Recurrent State-Space Models for Pick-and-Place Garment Flattening},
    author={Kadi, Halid Abdulrahim and Terzi{\'c}, Kasim},
    journal={arXiv preprint arXiv:2508.17070},
    year={2025}
  }
---
PS: The reported performance of the mesh-based planning method, [Visible Connectivity Dynamics (VCD)](https://sites.google.com/view/vcd-cloth), achieves 83% NI and 96% NC for T-shirt flattening in simulation and 50% NI and 68% NC in the real world within 20 steps. The improved method, [MEDOR](https://sites.google.com/view/occlusion-reason/home), achieves an NI above 80% across all tested garments in simulation within 10 steps, as well as 64% NI for trousers and 46.8% NI for dresses in real-world experiments within 10 steps.
{: .note-text}
