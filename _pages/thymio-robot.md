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

<div style="margin: 2rem 0;">
  <iframe 
    src="https://drive.google.com/file/d/12JovnytnGXysf7drYBUTP0FnLpmFwXlm/view?usp=drive_link" 
    width="100%" 
    height="480" 
    allow="autoplay"
    style="border: none; border-radius: 8px;">
  </iframe>
</div>

Built a complete autonomous navigation system for a Thymio robot as part of the EPFL Basics of Mobile Robotics course. The system detects the robot's pose from an overhead camera, plans an optimal path through a mapped environment using A* and navigates to the goal with real-time 3D obstacle avoidance.
State estimation combines camera observations and wheel odometry through an Extended Kalman Filter, keeping the robot localized even when the camera is temporarily unavailable.
