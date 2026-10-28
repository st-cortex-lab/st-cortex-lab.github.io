---
layout: project
title: DRAPER
subtitle: Towards a Robust Robot Deployment and Reliable Evaluation for Quasi-Static Pick-and-Place Cloth-Shaping Neural Controllers
venue: IEEE CASE 2025
authors: Halid Abdulrahim Kadi, Jose Alex Chandy, Luis Figueredo, Kasim Terzić, Praminda Caleb-Solly
affiliation: University of St Andrews and University of Nottingham
links:
  - { label: Paper, url: "https://doi.org/10.1109/CASE58245.2025.11163865" }
  - { label: arXiv, url: "https://arxiv.org/abs/2409.15159" }
  - { label: Benchmarks and Oracles, url: "https://github.com/halid1020/softgym-deepcloth" }
  - { label: Robot Control Scripts, url: "https://github.com/halid1020/robot_control_cloth" }
  - { label: Diffusion Policy, url: "https://github.com/halid1020/agent-arena-v0/tree/main/agent_arena/agent/bc/diffusion" }
  - { label: Configurations, url: "https://github.com/halid1020/agent-arena-v0/tree/main/agent_arena/configuration/train_and_evaluate/diffusion_policy" }
teaser:
  - { src: 01.jpg }
video: /assets/video/draper.mp4
abstract: >-
  Comparing robotic cloth-manipulation systems in a real-world setup is challenging. The fidelity gap between simulation-trained cloth neural controllers and real-world operation hinders the reliable deployment of these methods in physical trials. Inconsistent experimental setups and hardware limitations among different approaches obstruct objective evaluations. This study demonstrates a reliable real-world comparison of different simulation-trained neural controllers on both flattening and folding tasks with different types of fabrics varying in material, size, and colour. We introduce the DRAPER framework to enable this comprehensive study, which reliably reflects the true capabilities of these neural controllers. It specifically addresses real-world grasping errors, such as misgrasping and multilayer grasping, through real-world adaptations of the simulation environment to provide data trajectories that closely reflect real-world grasping scenarios. It also employs a special set of vision processing techniques to close the simulation-to-reality gap in the perception. Furthermore, it achieves robust grasping by adopting a tweezer-extended gripper and a grasping procedure. We demonstrate DRAPER's generalisability across different deep-learning methods and robotic platforms, offering valuable insights to the cloth manipulation research community.
bibtex: |
  @inproceedings{kadi2025draper,
    title={DRAPER: Towards a Robust Robot Deployment and Reliable Evaluation for Quasi-Static Pick-and-Place Cloth-Shaping Neural Controllers},
    author={Kadi, Halid Abdulrahim and Chandy, Jose Alex and Figueredo, Luis and Terzi{\'c}, Kasim and Caleb-Solly, Praminda},
    booktitle={2025 IEEE 21st International Conference on Automation Science and Engineering (CASE)},
    pages={3532--3539},
    year={2025},
    organization={IEEE}
  }
---
