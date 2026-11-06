---
title: "Variable-Stiffness Robotic Gripper for Food Handling"
excerpt: "Designed, fabricated, and experimentally validated a gripper that changes its grip force with temperature, for handling food items with very different physical properties. First-author publication at ICAROB 2024."
collection: portfolio
header:
  teaser: osaka-gripper/osaka-gripper-teaser.png
---

**Problem:** Automated food handling is difficult because food items vary in size, texture, 
weight, and fragility, sometimes within the same batch. Many food grippers either need the 
item's size or height known in advance, or need a specific grip force chosen ahead of time, 
which limits them when they meet items they haven't seen before.

**My contribution:** Working in the Harada Lab at Osaka University, I designed a gripper whose 
fingers use a temperature-dependent variable-stiffness fabric. Changing the temperature, rather 
than the mechanism or control scheme, changes how much force the gripper applies:

- **Warm (67 °C):** the fabric becomes compliant and applies gentle force, for soft, fragile, 
slippery, or heavy items
- **Cool (30 °C):** the fabric stiffens and applies more force, for hard or rigid items

I designed the gripper geometry in CAD, 3D printed the base, and sewed and pre-tensioned the 
fabric so it holds its curved shape even when softened. The curved base leaves a 2 mm gap 
between the fabric and base, guiding the fabric underneath items so the gripper can pick up 
flat, low-profile foods without them slipping through.

I then ran two sets of experiments:

1. **Force characterization** at two temperatures and three displacements (10, 20, 30 mm). 
The cooler fabric applied more force at every displacement; at 30 mm, peak force was 9.6 N 
cool versus 3.8 N warm. Force rose with displacement following a strong linear/quadratic 
trend (R² = 0.89–0.98), then dropped to a lower steady value once the fabric conformed to 
the object.
2. **Food picking** with 8 items chosen to be heavy, slippery, fragile, flat, or rigid, picked 
one at a time, from stacks, and in combined sequences, with the gripper mounted on an 
industrial robot using a depth camera for item localization and force feedback for closing.

**Result:** All eight food items were successfully grasped and transported. The failed 
attempts came from grasp-position misalignment (item off-centre, or grasp height mismatched 
to item height) rather than from the gripper itself, and items close to the gripper's minimum 
width were held less securely, pointing to adjustable finger width as the next design step.

**Tools:** CAD (Fusion 360), 3D printing, force gauge testing, Python

**[Paper: "Robotic Food Handling Utilizing Temperature Dependent Variable-Stiffness Material" (ICAROB 2024)](https://alife-robotics.co.jp/members2024/icarob/data/html/data/OS/OS14-2.pdf)**