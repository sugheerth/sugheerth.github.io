---
layout: page
title: Projects
permalink: /projects/
description: Selected robotics and autonomy research projects.
nav: true
nav_order: 3
---

<style>
  .project-stack {
    display: grid;
    gap: 3rem;
  }

  .project-stack__item {
    border-bottom: 1px solid var(--global-divider-color);
    padding-bottom: 3rem;
  }

  .project-stack__item:last-child {
    border-bottom: 0;
  }

  .project-stack__title {
    margin-bottom: 0.35rem;
  }

  .project-stack__description {
    color: var(--global-text-color-light);
    margin-bottom: 1.25rem;
  }

  .project-stack__media {
    margin: 1.25rem 0;
  }

  .project-stack__video-grid {
    display: grid;
    gap: 1rem;
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .project-stack video,
  .project-stack img {
    background: #fff;
    width: 100%;
  }

  .project-stack__caption {
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    margin: 0.5rem 0 0;
    text-align: center;
  }

  @media (max-width: 767px) {
    .project-stack__video-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="project-stack">
  <article class="project-stack__item">
    <h2 class="project-stack__title">EARTH</h2>
    <p class="project-stack__description">Excavation Autonomy with Resilient Traversability and Handling</p>
    <div class="project-stack__media">
      <video autoplay muted loop playsinline controls class="img-fluid rounded z-depth-1">
        <source src="{{ '/assets/video/earth-excavator-intro.mp4' | relative_url }}" type="video/mp4">
      </video>
    </div>
    <p>EARTH is a framework for autonomous excavators and earth-movers that integrates perception, planning, safe control, hydraulic actuation, and field deployment for embodied construction autonomy.</p>
    <p><a class="btn btn-sm btn-primary" href="https://droneslab.github.io/EARTH/" target="_blank" rel="noopener noreferrer">Full project page</a></p>
  </article>

  <article class="project-stack__item">
    <h2 class="project-stack__title">Safe Control with CLF-CBF-QP</h2>
    <p class="project-stack__description">Reactive safe planning for excavator-arm operation</p>
    <div class="project-stack__media project-stack__video-grid">
      <figure>
        <video autoplay muted loop playsinline controls class="img-fluid rounded z-depth-1">
          <source src="{{ '/assets/video/safe-planning-excavator-arm.mp4' | relative_url }}" type="video/mp4">
        </video>
        <figcaption class="project-stack__caption">3-DoF arm planning in a 2D state space with a single obstacle</figcaption>
      </figure>
      <figure>
        <video autoplay muted loop playsinline controls class="img-fluid rounded z-depth-1">
          <source src="{{ '/assets/video/safe-planning-3d-space.mp4' | relative_url }}" type="video/mp4">
        </video>
        <figcaption class="project-stack__caption">2-DoF arm planning in a 3D state space with multiple obstacles</figcaption>
      </figure>
    </div>
    <p>Safe planning mitigates risks associated with human injury, equipment damage, and environmental harm while enforcing constraints on key operating parameters. Control Lyapunov and Control Barrier functions support reactive planners that respond to obstacles before potential collisions occur.</p>
    <p><a class="btn btn-sm btn-primary" href="https://droneslab.github.io/EARTH/" target="_blank" rel="noopener noreferrer">Related EARTH page</a></p>
  </article>

  <article class="project-stack__item">
    <h2 class="project-stack__title">A Trajectory-Level Constraint Aware Framework For Safe Sampling</h2>
    <p class="project-stack__description">In progress - trajectory-level constraint-aware safe sampling</p>
    <div class="project-stack__media project-stack__video-grid">
      <video autoplay muted loop playsinline controls class="img-fluid rounded z-depth-1">
        <source src="{{ '/assets/video/sentinel-2d-maze.mp4' | relative_url }}" type="video/mp4">
      </video>
      <video autoplay muted loop playsinline controls class="img-fluid rounded z-depth-1">
        <source src="{{ '/assets/video/sentinel-pointmass-dense.mp4' | relative_url }}" type="video/mp4">
      </video>
    </div>
    <p>This work integrates a single smooth trajectory-level CBF correction into diffusion-based trajectory generation for fast, safety-aware planning in cluttered environments. The abstract examples show safe trajectory generation in Maze2D narrow-passage and PointMass2D dense-obstacle settings.</p>
    <p><strong>Status:</strong> In progress</p>
    <p><a class="btn btn-sm btn-primary" href="https://droneslab.github.io/SENTINEL/" target="_blank" rel="noopener noreferrer">Full project page</a></p>
  </article>

  <article class="project-stack__item">
    <h2 class="project-stack__title">Dynamics-Guided Trajectory Generation for Hydraulic Excavators</h2>
    <p class="project-stack__description">In progress - diffusion-based excavator trajectories with learned dynamics guidance</p>
    <div class="project-stack__media">
      {% include figure.liquid loading="eager" path="assets/img/dynamics-coherent-trajectory.png" title="Noisy and dynamically coherent excavator trajectories" class="img-fluid rounded z-depth-1" %}
    </div>
    <p>This ongoing work studies diffusion-based trajectory generation for hydraulic excavators with learned forward and inverse dynamics models. The diffusion model is to be trained on demonstrations simulated using the forward and inverse dynamics models. The sampler uses gradients from learned forward dynamics models for guidance during diffusion sampling to produce observation-control trajectories that are more dynamically coherent.</p>
    <div class="project-stack__media">
      {% include figure.liquid loading="eager" path="assets/img/trogen-x-workflow.png" title="Dynamics-guided diffusion workflow" class="img-fluid rounded z-depth-1" %}
    </div>
    <p><strong>Status:</strong> In progress</p>
    <p><a class="btn btn-sm btn-primary" href="https://droneslab.github.io/EARTH/#diffusion-trajectory-planning" target="_blank" rel="noopener noreferrer">Related EARTH section</a></p>
  </article>
</div>
