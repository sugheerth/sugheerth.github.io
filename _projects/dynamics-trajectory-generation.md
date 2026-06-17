---
layout: page
title: "Dynamics-Guided Trajectory Generation"
description: "In progress - diffusion-based excavator trajectories with learned dynamics"
img: assets/img/dynamics-coherent-trajectory.png
importance: 4
category: research
---

{% include figure.liquid loading="eager" path="assets/img/dynamics-coherent-trajectory.png" title="Noisy and dynamically coherent excavator trajectories" class="img-fluid rounded z-depth-1" %}

This ongoing work studies diffusion-based trajectory planning for hydraulic excavators with learned forward and inverse dynamics models. The planner uses dynamics guidance during sampling to generate observation-control trajectories that are more coherent with hydraulic actuation delays, valve dead zones, and machine-specific nonlinear dynamics.

{% include figure.liquid loading="eager" path="assets/img/trogen-x-workflow.png" title="Dynamics-guided diffusion workflow" class="img-fluid rounded z-depth-1" %}

<p><strong>Status:</strong> In progress</p>

<p><a class="btn btn-sm btn-primary" href="https://droneslab.github.io/EARTH/#diffusion-trajectory-planning" target="_blank" rel="noopener noreferrer">Related EARTH section</a></p>
