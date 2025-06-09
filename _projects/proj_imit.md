---
layout: page
title: Safety Guarantees in Imitation Learning
description: To design an online filter for the control inputs to avoid unsafe states, which improves iteratively
img: assets/img/barrier.png
importance: 4
category: research
related_publications: 
---
<i>Guide:</i> Prof. Florian Shkurti, University of Toronto.
- Conducted extensive literature survey on Lipchitz Neural Networks, the use of Normalizing Flows to learn stochastic differential equations and design of NN controllers for linear systems using Linear Matrix Inequalities
- Examined subspace projection techniques of learning dynamics to impose stability architecturally
- Recreated the results of in-Distribution Barrier Function (iDBF) on a custom toy problem
- Improved the safety framework of iDBF by generating contrastive distribution using Normalizing Flows
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/barrier.png" title="barrier function" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The barrier we were able to learn based on modifications to the in-Distribution Barrier Function
</div>