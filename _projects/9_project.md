---
layout: page
title: VIO based Navigation for a quadrotor
description: Development of planning, control, sensing and estimation stack for a quadrotor to navigate to a specified end goal
img: assets/img/quad_control/1.png
importance: 3
category: Classes
---


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/quad_control/1.png" title="Trajectory of quadrotor with VIO" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The goal of the project was to develop a complete planning and control system with state estimation
using visual inertial odometry (VIO) for a quadrotor, enabling it to fly from an initial point to a goal point
efficiently and without collision with obstacles or crashing. With perfect information of the state of the system
aggressive trajectories and controllers were feasible. With state estimation, however, aggressive trajectories
designed in prior projects are not feasible due to tracking errors in position and attitude of the quadrotor introduced
by the Visual Inertial Odometry(VIO) that is sensitive to themotion of the quad-rotor. Thus, this project aims to
outline the changes made in the trajectory generation and controls of the system,
in order for the quadrotor to perform well under the constraints introduced by state estimation.

Checkout the [code](https://github.com/harshg99/control_sensing_estimation_quadrotor) and the [report](/hgmain/assets/pdf/MEAM620_project3.pdf).
Checkout the video to see our quadrotor in action.

<iframe src="https://www.youtube.com/watch?v=j0pmaxFGDfY"
        width = "640"
        height = "480"
        frameborder="1"
        allowfullscreen>
</iframe>
