---
layout: page
title: Multi-robot mapping
description: Informative path planning for multi-robot mapping with Sampling based optimisation
importance: 5
img: assets/img/fyp/1.png
category: Research
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fyp/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>



Abstract: Autonomous mobile robots have evolved over the past 2 decades and have the
potential to change the way humans live and work. These robots can be made to
work autonomously in a diverse set of environments ranging from offices and
households to disaster sites and tough industrial environments. For autonomous
robots to be fully functional, robots would have to maintain an internal description
or a map of the environment to safely navigate through while carrying out the tasks
they are designed for.
The process of map building of an environment to extract relevant features is an
integral process for many robotics applications. Conventionally, these maps are
represented as discrete occupancy grids composed of cells that represent the
presence of an obstacle at a given location in the environment. In most of these
applications, an autonomous robot would have no prior information of the
environment it is placed within. Therefore, such a robot is initially tasked to explore
the environment to map features such as obstacles, walls and empty space.
Thus, the primary objective of this project is to propose a new exploration strategy
for building a map of an unknown environment. In the following section, we
provide a summary and review some of the exploration algorithms in literature.

The paths planned by this approach:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fyp/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Find out the [report](/hgmain/assets/pdf/fypreport.pdf) and the [code](https://github.com/harshg99/CMAES-Mapper).

