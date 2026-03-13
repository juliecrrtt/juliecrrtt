---
layout: single
title: "Megakaryocyte Detection – EPFL & CHUV"
permalink: /mk-detection/
author_profile: false
classes: wide mk-fullwidth
---

<a href="/juliecrrtt/" class="back-link">← Back to Portfolio</a>

<div class="project-card-horizontal">
  <img src="{{ '/assets/images/mk.jpeg' | relative_url }}" alt="Megakaryocyte detection" style="max-width: 200px; height: auto;">
  <div class="project-detail-meta">
    <p><strong>Period:</strong> Autumn 2025</p>
    <p><strong>Context:</strong> EPFL × CHUV collaborative project</p>
    <p><strong>Tools:</strong> QuPath, Cellpose, StarDist, ANN classifiers, DBSCAN</p>
    <a href="https://github.com/juliecrrtt/MK-project" class="github-btn" target="_blank">
      View on GitHub ↗
    </a>
  </div>
</div>



Built an automated pipeline for detecting and analyzing megakaryocytes (cells) in bone marrow histopathology slides, conducted as a Master's semester project at EPFL in collaboration with CHUV. 

The pipeline integrates deep-learning based segmentation (**Cellpose** for cell segmentation, **Stardist** for nuclear detection) with a custom **ANN pixel classifier** for bone structure segmentation.

Each detected cell is characterized by quantitative morphological and spatial features (area, nuclear lobulation, clustering via DBSCAN, distance to bone) implemented based on qualitative clinical tables. 

The complete system was deployed as a QuPath extension featuring one-click execution, interactive feature visualization and display of extracted cell features, making the analysis accessible to non-programming clinical users. 

