---
layout: page
title: Control for quadrotor
description: Leveraging differential flatness based control planners to learn  goal conditioned control policies for a quadrotor via reinforcement learning
img: assets/img/quad_control_gcrl/1.png
importance: 3
category: Research
---


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/quad_control_gcrl/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


This is an ongoing research project from my masters dissertation. The motion planning and control stack for quadrotors comprises of a trajectory planning phase
where given a sequence of waypoints a reference trajectory is planned leveraging the differential flatness property of quadrotors. Differential flatness leverages the
dynamical proporties of a system to represent the full state of the system in terms of specific variables and its derivatives. For a quadrotor, flat outputs comprise of the
position and yaw along the body frame z axis. Trajectories represented as polynomials in time are therefore planned in flat space. Given this reference trajectory, a cascading
PID controller is designed which controls attitude at a higher natural frequency than position.

However, since the planning phase is open loop and isn't informed of the limitations of the lower level PID controller,there are several problems that occur when tuning controllers
for specific trajectories. This is where goal conditioned reinforcement learning is useful, where a controller is directly synthesized to reach a goal without having to go through
the trajectory planning phase. This project intends to devise a curriculum to train an RL policy for a quadrotor to reach specified goals in flat space.

Find out the technical details in my [thesis](/hgmain/assets/pdf/penn_thesis).
