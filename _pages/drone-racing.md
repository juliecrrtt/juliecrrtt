---
layout: single
title: "Autonomous Drone Racing"
permalink: /drone-racing/
author_profile: false
classes: wide mk-fullwidth
---

<a href="/juliecrrtt/" class="back-link">← Back to Portfolio</a>
<div class="project-card-horizontal">
  <img src="{{ '/assets/images/drone.png' | relative_url }}" alt="Drone Racing" style="max-width: 200px; height: auto;">
  <div class="project-detail-meta">
    <p><strong>Period:</strong> Spring 2025</p>
    <p><strong>Context:</strong> EPFL course project</p>
    <p><strong>Tools:</strong> Computer Vision, PID Control, Trajectory Tracking</p>
  </div>
</div>


<div style="display: flex; gap: 2rem; align-items: flex-start; margin: 2rem 0;">
  <div style="flex: 1; min-width: 0;">
    <video width="100%" controls style="border-radius: 8px;">
      <source src="{{ '/assets/videos/video-simu-drone.mp4' | relative_url }}" type="video/mp4">
    </video>
  </div>
  <div style="flex: 1;">
    <p>Developed an autonomous navigation pipeline for a Crazyflie quadrotor to complete a course gate as fast as possible.</p>
    <p>In simulation (Webots), implemented a computer vision-based gate detection during the 1st lap using OpenCV, followed by high-speed trajectory tracking once gate positions were identified.</p>
    <p>Designed and tuned PID controller to ensure stable flight through randomly placed gates.</p>
  </div>
</div>

Transfered and retuned the algorithms from simulation to real Crazyflie hardware.  
