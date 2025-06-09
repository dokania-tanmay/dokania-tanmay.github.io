---
layout: page
title: Learning Set Representation using Kernel Functions
description: Given in-samples and out-samples, generate a function whose level set gives a boundary between them.
img: assets/img/zbf.png
importance: 1
category: research
related_publications: 
---
Guide: [Prof. Patricio Vela](https://scholar.google.com/citations?user=qL6ycTgAAAAJ&hl=en), Georgia Institute of Technology.

- Developed new theoretical guarantees for existence of a solution for hard-in and hard-out case.
- Implemented a algorithm in C++ that generates points and computes representation for a keyhole in 11ms.
- Extended the formulation to sets in SE(2) and demonstrated utility for representation of reachable poses for end-effector.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/zbf.png" title="Keyhole Level-set Representation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Generation of in- and out-samples, followed by the linear optimization problem to obtain the level representation.
</div>

*This project is still in-progress.*