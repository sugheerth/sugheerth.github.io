---
layout: page
title: "Safe Control with CLF-CBF-QP"
description: "Reactive safe planning for excavator-arm operation"
img: assets/img/safe-planning.png
importance: 2
category: robotics
---

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    <video autoplay muted loop playsinline controls class="img-fluid rounded z-depth-1">
      <source src="{{ '/assets/video/safe-planning-excavator-arm.mp4' | relative_url }}" type="video/mp4">
    </video>
    <p class="text-center text-muted mt-2">3-DoF arm planning in a 2D state space with a single obstacle</p>
  </div>
  <div class="col-sm mt-3 mt-md-0">
    <video autoplay muted loop playsinline controls class="img-fluid rounded z-depth-1">
      <source src="{{ '/assets/video/safe-planning-3d-space.mp4' | relative_url }}" type="video/mp4">
    </video>
    <p class="text-center text-muted mt-2">2-DoF arm planning in a 3D state space with multiple obstacles</p>
  </div>
</div>

This project uses CLF-CBF-QP based control to enforce safety and stability constraints for excavator-arm motion, with the goal of avoiding collisions while maintaining efficient task execution.

<p><a class="btn btn-sm btn-primary" href="https://droneslab.github.io/EARTH/" target="_blank" rel="noopener noreferrer">Related EARTH page</a></p>
