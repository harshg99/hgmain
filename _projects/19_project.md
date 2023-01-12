---
layout: page
title: Teleoperation
description: Software integration of teleoperative device with a robotic arm ad soft gripper to provide expert demonstrations
importance: 2
img : assets/img/teleop/2.png
category: Fun
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/teleop/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

This was a fun summer project in 2018 alongside my intership where the objective was to collect expert demonstrations for assembly tasks via a Denso robotic arm and soft gripper.
My role in the project was to develop the engineering pipeline to collect such data. We used a 7-DOF Force Dimension Haptic Device for remote teleoperation of a Denso robotic arm.
The necessary end effector torques on the robotic arm are converted to the reactive forces on the haptic device. Furthermore,
there is a forward and inverse kinematics tool transcribed to do this conversion in real-time.

The programming of the robot was done on Matlab Simulink using simple Inverse Kinematics and Dynamics.

The video for teleoperation can be found here


<iframe src="https://youtu.be/OW81gdqCgDk"
        width = "640"
        height = "480"
        frameborder="1"
        allowfullscreen>
</iframe
