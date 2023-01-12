---
layout: page
title: Safe Exploration
description: Safe exploration while learning control policies for an autonomous vehicle with Reinforcement Learning
importance: 1
category: Classes
---


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/quad_control_gcrl/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


Exploration for Reinforcement Learning is a well-addressed problem in the research community.
However, for many robotics tasks, certain states are infeasible to explore due to state constraints
imposed by obstacles or robot design. Some of the earlier work on exploration has been restricted
to the bandit setting without safety constraints. Hence, this project attempts to do a literature
review on safe exploration with reinforcement learning for real robotics tasks and we attempt to
experiment with some of the recent methods for safe exploration. The primary objective of this
problem is to achieve high long-term reward, i.e., low regret while satisfying safety constraints with
high probability when the dynamics of the underlying process is not completely known. Here the
objective is twofold. First, our algorithm should take actions that drive our agent towards high long-
term rewards. Since the underlying dynamics of the agent are not completely known in our problem,
our agent should not take spurious actions that make it unsafe.

Inspired by recent developments, we aim to further study safe exploration in the context of non
tabular robotics tasks where we would attempt to answer questions on the regret bounds in tasks
with continuous actions. We do this for a safe navigation task in an autonomous vehicle.
We attempt to present theoretical analysis on the regret bounds for different algorithms
with continuous action spaces. We also implement and analyze the performance of a safe
exploration algorithm on the autnomous vehicle environment.
