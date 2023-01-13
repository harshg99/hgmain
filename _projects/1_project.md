---
layout: page
title: Traffic Signal Control
description: Distributed traffic signal control with multi-agent reinforcement learning
img: assets/img/tsc/1.png
importance: 1
category: Research
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/tsc/1.png" title="Multi Agent Tracking" class="img-fluid rounded z-depth-1" %}
    </div>
</div>



Autonomous driving is the future, however autonomy will only be beneficial to society if vehicles and infrastructure can coordinate with each other to reduce traffic congestion and
improve travel times. Intelligent decision making on the infrastructure side (e.g., traffic signals) is of paramount importance to regulate traffic flow. However, centralized control
of the traffic infrastructure is infeasible, and in large metropolis that can count upwards of thousands of junctions, and decentralization will be necessary.

This research was aimed at intelligent decision making for traffic signal control based on the traffic conditions at a junction (i.e number and speed of incoming vehicles,
queue lengths,etc,) as well as the conditions of adjacent junctions. We use distributed reinforcement learning approaches to tackle the coordination problem. In particular, how do
agents learn to coordinate traffic flow with their neighbors such that the ensuing behavior of an agent to cooperate results in citywide traffic flow improvements.

Checkout out our recent full paper accepted to AAMAS 2023 for more details,


