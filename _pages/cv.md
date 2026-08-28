---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. in Mechanical Engineering (Robotics, Control, Autonomous Systems), San Diego State University, 2024
* B.S. in Mechatronics, Robotics and Automation Engineering, California State University, Chico, 2018

Work experience
======
* Aug 2021 - May 2024: Graduate Research Assistant III
  * San Diego State University, DSIM Lab
  * Led development of an adaptive control approach — extremum seeking control (ESC) — implemented in ROS2 for mobile robot motion, enabling a robot with no prior knowledge of its environment to locate a signal source (light or sound) via real-time continuous optimization
  * Actuated a sensor on a servo to widen local search, achieving faster and more energy-efficient convergence (~1000% improvement) compared to prior methods

* Aug 2021 - May 2024: Teaching Assistant
  * San Diego State University
  * Systems Modeling & Analysis (Spring '24) and Robot Modeling & Control (Fall '23) — see [Teaching](/teaching/) for details

* Freelance: Course Designer
  * The Construct
  * Optimized and debugged ROS2 and Gazebo simulation environments for robotics education
  * Designed and implemented a CNN-based image recognition system for a simulated security robot, integrating computer vision with ROS2 perception and decision-making pipelines

* Apr 2019 - Mar 2022: Field Engineer II
  * Honeywell Process Solutions, San Bruno, CA
  * Principal technical expert for HVAC and commercial Fire Alarm, Security, and Access Control systems
  * Programmed building management controls in Honeywell software; led startup troubleshooting and mentored junior field service representatives

Skills
======
* Robotics: ROS2, Gazebo, TurtleBot3, sensor/actuator integration, kinematics & dynamics
* Controls & Optimization: Extremum seeking control, adaptive control, linear programming (duality, simplex method), Gurobi
* Computer Vision & Deep Learning: CNNs, image classification, perception pipelines
* Software: Python, C++, MATLAB, Git
* CAD & Fabrication: Onshape, 3D printing
* Other: Technical writing, teaching, mentoring, leadership

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
