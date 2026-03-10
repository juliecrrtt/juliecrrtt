---
layout: single
permalink: /
author_profile: true
show_title: false
show_permalink: false
---

Welcome to my GitHub portfolio! Here, I showcase my academic projects.

---

## Education
- Master in Robotics – EPFL, 2nd year
- Bachelor in Microengineering – EPFL 

---

## Key Projects


<div class="project-card-horizontal" onclick="toggleCard(this)" role="button" tabindex="0" aria-expanded="false">

  <img src="{{ '/assets/images/mk.jpeg' | relative_url }}" 
       alt="Megakaryocyte detection">

  <div class="project-content">
    <h3>
      <a href="https://github.com/juliecrrtt/MK-project" onclick="event.stopPropagation()">
        Megakaryocyte Detection – EPFL & CHUV
      </a>
    </h3>

    <p><strong>Autumn 2025</strong></p>

    <p>
      QuPath extension for automated detection and morphology analysis of megakaryocytes.
    </p>

    <p>
      <strong>Tools:</strong> Cellpose, StarDist, ANN classifiers, DBSCAN
    </p>

    <div class="more-details">
      <p>
        Built pipelines using <strong>Cellpose</strong> for deep learning-based cell segmentation.  
        Implemented nucleus and osteostructure detection using <strong>StarDist</strong> and <strong>ANN pixel classifiers</strong>.  
        Developed quantitative MK morphology metrics: cell area, clustering patterns (DBSCAN), lobulation, and distance to bone structures.  
        Enabled automated, reproducible analysis to support clinical research on bone marrow tissue.
      </p>
    </div>

    <span class="card-hint">Click to expand ▾</span>

  </div>

</div>

---

### [Multimodal Machine Learning for Species Distribution Modeling - EPFL](#)
**Autumn 2025**  
Built a **multimodal machine learning pipeline** combining climatic variables, **Landsat time series**, and **Sentinel-2 imagery** to predict the presence of **342 plant species**, as part of the course *Image Processing for Earth Observation*.  

---

### [Chocolate Recognition (Deep Learning) - EPFL](#)
**Spring 2025**  
Developed a **CounterResNet model** with **synthetic data augmentation**, achieving an **F1 score of 0.91**, as part of the course *Image Analysis for Pattern Recognition*.  

--- 

### [Thymio Robot (EKF Localization) - EPFL](#)  
**Autumn 2025**<br>
Estimated the **position of a Thymio robot** using an **Extended Kalman Filter (EKF)** with or without camera measurements. Tested performance across multiple trajectories, speeds, and angular velocities derived from wheel encoders to evaluate **localization accuracy**.  


<script>
function toggleCard(card) {
  const details = card.querySelector('.more-details');
  const hint = card.querySelector('.card-hint');
  const isOpen = card.classList.contains('is-open');

  if (isOpen) {
    details.style.display = 'none';
    hint.textContent = 'Click to expand ▾';
    card.classList.remove('is-open');
    card.setAttribute('aria-expanded', 'false');
  } else {
    details.style.display = 'block';
    hint.textContent = 'Click to collapse ▴';
    card.classList.add('is-open');
    card.setAttribute('aria-expanded', 'true');
  }
}

// Allow keyboard activation (Enter / Space)
document.querySelectorAll('.project-card-horizontal').forEach(card => {
  card.addEventListener('keydown', e => {
    if (e.key === 'Enter' || e.key === ' ') {
      e.preventDefault();
      toggleCard(card);
    }
  });
});
</script>
