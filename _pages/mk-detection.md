---
layout: single
title: "Megakaryocyte Detection – EPFL & CHUV"
permalink: /mk-detection/
author_profile: false
classes: wide
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



## Overview

Developed a **QuPath extension** for automated **detection and analysis of megakaryocytes (MK)** in bone marrow histopathology slides.

---

## Pipeline

### 1. Cell Segmentation - Cellpose
Built deep learning-based segmentation pipelines using **Cellpose** to detect and outline individual megakaryocytes from whole-slide images, handling variable staining and cell sizes.

### 2. Nucleus & Structure Detection - StarDist & ANN
- **nucleus detection** using **StarDist**.
- **osteostructures segmentation** using an **ANN pixel classifier** trained on custom annotations.

### 3. Morphology Metrics
Developed a suite of quantitative descriptors per detected MK:

| Metric | Description |
|---|---|
| **Cell area** | Surface area of each MK |
| **Lobulation** | Nuclear lobulation index |
| **Clustering (DBSCAN)** | Spatial grouping of MKs in the marrow |
| **Distance to bone** | Proximity of each MK to bone structures |

## Extension & Clinical Integration
The entire pipeline was integrated as a **fully deployable QuPath extension**, enabeling high accessibility for non-programming users.

Key features include:

- **One-click execution** of the full analysis pipeline  
- Automated computation of morphological and spatial metrics  
- Interactive visualization of the detections  
- Structured data export (tables + annotations) for downstream statistical analysis  

