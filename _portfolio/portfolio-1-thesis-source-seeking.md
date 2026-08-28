---
title: "Thesis: TurtleBot3 Sensor-Actuated Source Seeking"
excerpt: "Servo-actuated extremum seeking control for source localization on a nonholonomic robot.<br/><img src='/images/rotating-frame.png'>"
collection: portfolio
---

My master's thesis explored applying extremum seeking control (ESC) — an adaptive control approach — to real robots and simulations, with a focus on source-seeking behavior.

The robot used was a TurtleBot3 from Robotis, a nonholonomic robot capable of moving forward along the x-axis and rotating about the z-axis. Its modular design allowed for custom additions, including an extra servo motor for a rotating sensor. This sensor moves back and forth to estimate the location of a signal source — light or sound in our tests — enabling local exploration that computes the derivative of the signal and perturbs the vehicle's motion toward the source.

The robot has no prior knowledge of the exact source location; it only receives gradient estimates derived from sensor data as it approaches within roughly 0.5 meters of the source.

The project spanned three phases: theoretical research and analysis, simulation in Gazebo/ROS2 to validate the theory, and physical robot construction for real-world testing. Custom hardware (a top layer and rotating arm for the sensor) was modeled in Onshape and 3D-printed on a Bambu H2S. The physical robot used a Raspberry Pi 4 for onboard compute, with a microphone and photoresistor as sensors.

Using parameters tuned in simulation, the robot successfully converged to the source based on both light and sound detection in real-world testing — the basis for the resulting [publication](/publications/).

**Skills:** Git, Python, C++, autonomous systems, adaptive control, optimization, robotics, ROS2, leadership

<img src='/images/light-source.png'>
<img src='/images/rotating-frame.png'>

[Watch the demo video](https://www.youtube.com/watch?v=K2YwE-z4ytc)
