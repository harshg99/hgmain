---
layout: page
title: Informative Path Planning
description: Informative Path Planning for aerial vehicles in target classification and semantic segmentation tasks with Reinforcement Learning
importance: 4
img: assets/img/ipp/1.png
category: Research
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ipp/2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Abstract -  Active target sensing is the task of discovering and
classifying an unknown number of targets in an environment
and is critical in search-and-rescue missions. This paper develops a deep reinforcement learning approach to plan informative
trajectories that increase the likelihood for an uncrewed aerial
vehicle (UAV) to discover missing targets. Our approach efficiently (1) explores the environment to discover new targets, (2)
exploits its current belief of the target states and incorporates
inaccurate sensor models for high-fidelity classification, and (3)
generates dynamically feasible trajectories for an agile UAV by
employing a motion primitive library. Extensive simulations on
randomly generated environments show that our approach is
more efficient in discovering and classifying targets than several
other baselines. A unique characteristic of our approach, in
contrast to heuristic informative path planning approaches, is
that the it is robust to varying amounts of deviations of the
prior belief from the true target distribution, thereby alleviating
the challenge of designing heuristics specific to the application
conditions.

Find out the [code](https://github.com/harshg99/informative_path_planning_quads).

