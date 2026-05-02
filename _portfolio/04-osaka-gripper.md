---
title: "Variable-Stiffness Robotic Gripper for Food Handling"
excerpt: "Designed, fabricated, and experimentally validated a temperature-dependent variable-stiffness end-effector for grasping food items with diverse physical properties. First-author publication at ICAROB 2024."
collection: portfolio
---

**Problem:** Automated food handling is difficult because food items vary in size, texture, 
weight, and fragility — sometimes within the same batch. Most gripper designs either apply 
fixed force (damaging soft items) or require predetermination of item geometry (impractical 
at scale).

**My contribution:** I designed a gripper that uses a temperature-dependent variable-stiffness 
fabric on the finger surfaces. By controlling temperature rather than mechanical configuration, 
the gripper adapts its compliance without complex control procedures:

- **Hot mode:** fabric becomes compliant, applying gentle force — for fragile, soft, or 
slippery items
- **Cold mode:** fabric stiffens, applying greater force — for heavy or rigid items

I designed the full gripper geometry in CAD, 3D printed the base structure, attached and 
pre-tensioned the fabric, and conducted two validation experiments:

1. **Force gauge characterization** across two temperatures and three displacement values, 
confirming a second-order polynomial force-displacement relationship and inverse proportionality 
between force and temperature
2. **Food picking experiments** with 8 food items spanning heavy, slippery, fragile, brittle, 
flat, and rigid categories — in sequential, stacked, and combined arrangements

The gripper was integrated with an industrial robot using a depth camera for item localization 
and force feedback for grasp closure.

**Result:** Successful grasp and transport of all food categories without damage. Published at 
the International Conference on Artificial Life and Robotics (ICAROB 2024), Osaka University.

**Tools:** CAD (Fusion 360), 3D printing, force gauge, industrial robot integration, Python

**[Paper — ICAROB 2024](https://alife-robotics.co.jp/members2024/icarob/data/html/data/OS/OS14-2.pdf)**
