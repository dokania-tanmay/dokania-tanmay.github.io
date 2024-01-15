---
layout: page
title: Guidance and Control Laws in Three Body Pursuit
description: Designing controller for two teams- one with an attacker and the other with a target and defender. 
img: assets/img/tad.png
importance: 3
category: course
related_publications: 
---
Guide: [Prof. Dwaipayan Mukherjee](https://www.ee.iitb.ac.in/web/people/dwaipayan-mukherjee/), IIT Bombay.
- Developed strategies for an attacking missile to capture a target while evading a defender missile
- Formulating the problem as a safety-critical system with the application of Zeroing and Reciprocal Control Barrier functions to guarantee safety from the defender
- Developing new guidance law which maximizes performance and ensures safety using quadratic programming after analysis of existing and widely used laws for missile guidance
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/tad.png" title="simulation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Controller simulation based on safety constraints inforced using a barrier function and solved as an quadratic program.
</div>