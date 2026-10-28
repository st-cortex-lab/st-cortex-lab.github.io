---
layout: project
title: JA-TN
subtitle: Pick-and-Place Towel Shaping from Crumpled States based on TransporterNet with Joint-Probability Action Inference
venue: CoRL 2024
authors: Halid Abdulrahim Kadi and Kasim Terzić
affiliation: University of St Andrews
links:
  - { label: Paper, url: "https://proceedings.mlr.press/v270/kadi25a.html" }
  - { label: OpenReview, url: "https://openreview.net/forum?id=SW8ntpJl0E" }
  - { label: Benchmarks and Oracles, url: "https://github.com/halid1020/softgym" }
  - { label: Method, url: "https://github.com/halid1020/agent-arena-v0/tree/main/agent_arena/agent/bc/transporter" }
  - { label: Configurations, url: "https://github.com/halid1020/agent-arena-v0/tree/main/agent_arena/configuration/train_and_evaluate/ja-tn" }
abstract: >-
  Towel manipulation is a crucial step towards more general cloth manipulation. However, folding a towel from an arbitrarily crumpled state and recovering from a failed folding step remain critical challenges in robotics. We propose joint-probability action inference JA-TN, as a way to improve TransporterNet’s operational efficiency; to our knowledge, this is the first single data-driven policy to achieve various types of folding from most crumpled states. We present three benchmark domains with a set of shaping tasks and the corresponding oracle policies to facilitate the further development of the field. We also present a simulation-to-reality transfer procedure for vision-based deep learning controllers by processing and augmenting RGB and/or depth images. We also demonstrate JA-TN’s ability to integrate with a real camera and a UR3e robot arm, showcasing the method’s applicability to real-world tasks.
sections:
  - title: Method
    groups:
      - cols: 2
        items:
          - { src: 01.png, caption: JA-TN }
          - { src: 02.png, caption: Towel Shaping Tasks }
      - items:
          - { src: 03.png, caption: A Folding-from-crumpled Trajectory produced by JA-TN }
  - title: Simulation-to-Reality Transfer
    groups:
      - cols: 2
        items:
          - { src: 04.png, caption: Vision processing for Training }
          - { src: 05.png, caption: Vision processing for Real-World Deployment }
  - title: Benchmark Domains
    groups:
      - cols: 3
        items:
          - { src: 06.png, caption: Mono Square Fabrics }
          - { src: 07.png, caption: Rainbow Square Fabrics }
          - { src: 08.png, caption: Rainbow Rectangular Fabrics }
bibtex: |
  @inproceedings{kadi2024jatn,
    title={{JA-TN}: Pick-and-Place Towel Shaping from Crumpled States based on TransporterNet with Joint-Probability Action Inference},
    author={Kadi, Halid Abdulrahim and Terzi{\'c}, Kasim},
    booktitle={Proceedings of The 8th Conference on Robot Learning},
    series={Proceedings of Machine Learning Research},
    volume={270},
    pages={3107--3123},
    year={2025},
    publisher={PMLR}
  }
---
