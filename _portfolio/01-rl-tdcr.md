---
title: "Contact-Aware Navigation for Tendon-Driven Continuum Robots Using Reinforcement Learning"
excerpt: "Designed and trained a physics-based RL policy for a continuum robot to navigate 
cluttered environments by exploiting contact — outperforming a geometric baseline by 20 
percentage points."
collection: portfolio
header:
  teaser: images/rl-tdcr-env-top.png
---

**Problem:** Traditional motion planners for continuum robots treat contact as a failure 
condition. In cluttered or inspection environments this is too conservative — contact 
with obstacles is often unavoidable and can be exploited to reach otherwise inaccessible goals.

![MuJoCo simulation environment perspective view](/images/rl-tdcr-env-perspective.png)
![MuJoCo simulation environment top view](/images/rl-tdcr-env-top.png)

**My contribution:** This was a graduate course project (MIE1630) that I conceived and led. 
My specific contributions:

- **Project concept and direction** — proposed the contact-aware RL formulation and defined 
the problem structure
- **Reward engineering** — designed the potential-based reward shaping framework incorporating 
a contact-aware geometric cost-to-go heuristic, which proved essential: ablating it collapsed 
success rate from 60.5% to under 20%
- **Training and hyperparameter tuning** — ran all training experiments on GPU (SAC with 
cVAE + Mamba-2 policy architecture), managed the training pipeline and checkpoint selection
- **Evaluation** — conducted all policy evaluations across 1,621 held-out goal configurations, 
including spatial analysis, failure mode characterization, and contact subset breakdowns
- **Ablation study** — designed and ran the heuristic shaping ablation confirming its necessity

The policy architecture uses a conditional variational autoencoder (cVAE) with a Mamba-2 
sequence backbone trained under the Soft Actor-Critic (SAC) objective. The geometric baseline 
(A* over contact-aware lattice) was implemented by a teammate.

**Result:** The learned policy achieved 60.5% physical execution success across 1,621 held-out 
goal configurations under full MuJoCo physics, compared to 40.1% for the geometric baseline. 
The policy successfully threads narrow ~5 cm inter-obstacle corridors where kinematic plans 
fail under real physics — backbone compliance, friction, and actuator dynamics included.

![Success rate heatmap across workspace](/images/rl-tdcr-results.png)

<video controls playsinline preload="metadata" width="100%">
  <source src="https://rozmarco.github.io/files/videos/99.mp4" type="video/mp4">
  Your browser does not support HTML video.
</video>

  <div style="flex: 1 1 300px; min-width: 0;">
    <img src="/images/rl-tdcr/35_vid.png"
         alt="Planned robot trajectory through the environment"
         style="display: block; width: 100%; height: auto;">
  </div>

</div>

**Project presentation**
[View presentation in Google Slides](https://docs.google.com/presentation/d/1IU6Nf6CIuJABqPL0DOccSY2poR49zBh2R-pdnnPa9s/edit)

**Tools:** Python, MuJoCo, PyTorch, SAC, Gymnasium, Linux, CUDA
