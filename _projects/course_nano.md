---
layout: page
title: Nanosaur - Electronic Design Lab
description: Hazardous Gas Leakage Detection using Nanosaur and Jetson Nano.
img: assets/img/nano.jpg
importance: 1
category: course
related_publications: 
---
The aim of the project was to do modifications to [Nanosaur](https://nanosaur.ai/) by [Raffaello Bonghi](https://rnext.it/). We designed a custom Printed Circuit Board to mount the three gas sensors on Jetson Nano. We also designed a 3D-printed camera housing to mount a binocular camera with an integrated IMU. On the software front, we deployed [ORBSLAM-2](https://github.com/raulmur/ORB_SLAM2) on the hardware to do Visual-SLAM.

The high level idea was to use the data from gas sensors and localization from VSLAM to find locations with a higher gas concentration, which corresponds to regions close to the leakage. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/web_ss.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/slam.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/front_right_con.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
Please find details in our [GitHub repository.](https://github.com/dokania-tanmay/nanosaur_gas_detection)

We were awarded the Best Project Award for our work, and it was featured on [Wadhwani Electronics Laboratory's YouTube Channel!](https://youtu.be/vspevFlvx1A)

**Authors**: Tanmay Dokania, [Navneet](https://navneet-13.github.io/), [Aziz Shameem](https://aziz-shameem.github.io/)