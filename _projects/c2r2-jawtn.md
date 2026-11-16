---
layout: project
title: C2R²-JawTN
subtitle: Towards General Imitation Pick and Place with Parallel Grippers
venue: Preprint 2026
authors: Halid A. Kadi, Emily Pondaven, John Oyekan, Kasim Terzić, Juan Ye
affiliation: University of St Andrews and Loughborough University
links:
  - { label: "Paper (coming soon)", url: "#" }
  - { label: "Code (coming soon)", url: "#" }
abstract: >-
  Transporter Networks learn tabletop rearrangement from under 1000 demonstrations on PyBullet Ravens, whose robot holds a suction cup that grips anything at any angle and holds it as if welded. A real parallel jaw must choose its grasp angle and height, needs room beside the object and holds by friction alone. We ask how far imitation gets with a jaw and actual grasping, and contribute three things. JawRaven rebuilds Ravens' ten tasks in MuJoCo for a UR3e with a Robotiq Hand-E jaw and one overhead RealSense camera, as in our real cell, with one RGB-D input and one 8-number action for every task. Real-JawRaven writes every object as a printable part read back from the simulation, so that a simulated test episode can be set up on the real table. C2R²-JawTN is a coarse-to-fine Transporter for parallel grippers: it refines the pick and the place twice, through finer and turned crops, and learns both heights. One architecture, trained on 100 demonstrations per task, serves every task; the results below are generated from the same evaluations as the paper. We are currently conducting real-world training and experiments to further validate this approach in the real world.
sections:
  - title: JawRaven
    groups:
      - cols: 2
        items:
          - { src: 01.jpg, caption: "The cell: a UR3e with a Hand-E jaw, the overhead D435i's beam (yellow), the region the policy sees (red) and the half-ring the arm works in (blue)" }
          - { src: 02.jpg, caption: "What the policy is given and returns: the colour and height maps, and the action (the jaw at the pick in red, at the place in blue)" }
      - items:
          - { src: 03.jpg, caption: "The ten tasks: each start scene in PyBullet Ravens, then JawRaven's start and goal" }
          - { src: 04.jpg, caption: "Why assembling kits is harder: in Ravens the cup drops a piece over a painted outline; in JawRaven the jaw must fit it into a pocket with 4 mm of play" }
  - title: C2R²-JawTN
    groups:
      - items:
          - { src: 05.jpg, caption: "The architecture: a coarse Transporter, then two refinement levels on finer, turned crops, and a depth network for both heights; pick, key, query and place outputs each in their own colour" }
          - { src: 06.jpg, caption: "Every map the networks compute for one held-out kits step that places the letter G, level by level, to the final action" }
  - title: Real-JawRaven
    groups:
      - items:
          - { src: 07.jpg, caption: "Every object prints one to one from the simulation, in real filament colours" }
---

{% include c2r2_results.html %}
