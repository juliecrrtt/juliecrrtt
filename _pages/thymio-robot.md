---
layout: single
title: "Thymio robot"
permalink: /thymio-robot/
author_profile: false
classes: wide mk-fullwidth
---

<a href="/juliecrrtt/" class="back-link">← Back to Portfolio</a>
<div class="project-card-horizontal">
  <img src="{{ '/assets/images/thymio.png' | relative_url }}" alt="Thymio robot" style="max-width: 200px; height: auto;">
  <div class="project-detail-meta">
    <p><strong>Period:</strong> Autumn 2024</p>
    <p><strong>Context:</strong> EPFL course project</p>
    <p><strong>Tools:</strong> Computer Vision, EKF, Path Planning, Mobile Robotics</p>
  </div>
</div>

<div style="display: flex; gap: 2rem; align-items: flex-start; margin: 2rem 0;">
  <div style="flex: 1; min-width: 0;">
    <video width="100%" controls style="border-radius: 8px;">
      <source src="{{ '/assets/videos/Video_thymio.mp4' | relative_url }}" type="video/mp4">
    </video>
  </div>
  <div style="flex: 1;">
    <p>Built a complete autonomous navigation system for a Thymio robot as part of the EPFL _Basics of Mobile Robotics course_. The system detects the robot's pose from an overhead camera, plans an optimal path through a mapped environment using **A*** and navigates to the goal with real-time 3D **obstacle avoidance**.</p>
    <p>State estimation combines camera observations and wheel odometry through an **Extended Kalman Filter**, keeping the robot localized even when the camera is temporarily unavailable.</p>
  </div>
</div>
