---
title: "Open-Source Extensible Tendon-Driven Continuum Robot"
excerpt: "Designed, fabricated, and characterized a two-segment TDCR with a novel magnetically self-distributing extensible degree of freedom — with full open-source design files and assembly documentation."
collection: portfolio
---

**Problem:** Most continuum robot platforms lack an extensible degree of freedom, limiting 
their ability to navigate constrained spaces like pipes or surgical cavities without 
repositioning the base.

**My contribution:** I designed an extensible TDCR from scratch — CAD, fabrication, 
electronics integration, and teleoperation software. The key mechanical insight is using 
passive magnetic spacer disks that self-distribute during axial extension, avoiding active 
spacing mechanisms and additional actuators. The system uses a concentric tube-rod backbone 
with rail-mounted DYNAMIXEL actuation.

I also developed experimental protocols for workspace characterization, curvature measurement, 
and follow-the-leader performance evaluation, and contributed the platform to the Continuum 
Robotics Laboratory's open-source ecosystem.

**Result:** The robot successfully navigates planar and three-dimensional pipe-based task 
spaces using teleoperation, demonstrating that the extensible DOF allows end-effector 
advancement without base repositioning.

[![TDCR Demo](https://img.youtube.com/vi/u-8E7-xkPwE/0.jpg)](https://youtu.be/u-8E7-xkPwE)  
▶️ [Watch the demo](https://youtu.be/u-8E7-xkPwE)

**[GitHub — Full design files and assembly documentation](https://github.com/rozmarco/extensible_tdcr)**

**Tools:** SolidWorks / Fusion 360, DYNAMIXEL, Python, ROS2
