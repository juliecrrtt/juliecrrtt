---
layout: single
title: "Megakaryocyte Detection – EPFL & CHUV"
permalink: /mk-detection/
author_profile: false
classes: wide
---

<a href="/juliecrrtt/" class="back-link">← Back to Portfolio</a>

<div class="project-detail-header">
  <img src="/assets/images/mk.jpeg" alt="Megakaryocyte detection" class="project-detail-img">
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

Developed a **QuPath extension** for automated **detection and analysis of megakaryocytes (MK)** in bone marrow histopathology slides, enabling reproducible clinical research at CHUV.

---

## Pipeline

### 1. Cell Segmentation — Cellpose
Built deep learning-based segmentation pipelines using **Cellpose** to detect and outline individual megakaryocytes from whole-slide images, handling variable staining and cell sizes.

### 2. Nucleus & Structure Detection — StarDist & ANN
- Implemented **nucleus detection** using **StarDist**, a star-convex polygon model well-suited to round/oval nuclei.
- Applied **ANN pixel classifiers** to detect and segment surrounding **osteostructures** (bone trabeculae).

### 3. Morphology Metrics
Developed a suite of quantitative descriptors per detected MK:

| Metric | Description |
|---|---|
| **Cell area** | Surface area of each MK |
| **Lobulation** | Nuclear lobulation index |
| **Clustering (DBSCAN)** | Spatial grouping of MKs in the marrow |
| **Distance to bone** | Proximity of each MK to bone structures |

### 4. Output & Clinical Use
Results are exported as structured tables and overlay annotations within QuPath, enabling pathologists to review, validate, and use data directly in clinical research workflows.

---

## Key Challenges

- Handling **staining variability** across tissue slides
- Tuning **DBSCAN parameters** (ε, min_samples) for sparse vs. dense MK distributions
- Balancing **sensitivity vs. specificity** in nucleus vs. cytoplasm boundary detection

---

## Results

Achieved robust automated detection allowing **reproducible, high-throughput analysis** of bone marrow biopsies, reducing manual annotation time significantly.
