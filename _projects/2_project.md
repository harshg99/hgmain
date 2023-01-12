---
layout: page
title: Multi Agent Search and Tracking
description: Multi-agent reinforcement learning for persistent target tracking
img: assets/img/search/1.png
importance: 2
category: Research
---



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/search/2.gif" title="Multi Agent Tracking" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The problem of multi agent search and tracking encompasses a group of agents (pursuers) tracking a group of moving targets. This is especially useful in many surveillance applications in defence, environmental
monitoring and search and rescue. Most of these applications are geared towards large scale deployment and as such control policies for these agents must be fully decentralized to ensure scalability to different pursuer team sizes.

The primary objective in the problem is for a team of pursuers need to minimize the uncertainties in the estimates over the positions of the targets. Each pursuer has limited sensing and communication ability i.e. each agent can sense
and communicate within a given radius. Given the limitations in the sensing cabilities of any given pursuer,  what is a good control strategy for an individual agent to adapt such that they can synergise their motion, sensing and communication
capabilities to reduce their cumulative uncertainty over all targets in the environment.

In the problem setup, each individual agent is equipped with a range sensor that can detect a target with perfect precision. Both agents and targets are modelled with SE2 dynamics where the control policy is unknown and stochastic. Since the targets are moving,
an Unscented Kalman Filter is used to estimate the uncertainty in the position of the targets. Agents can communicate and merge their beliefs once in range. The control policies are learnt with multi-agent reinforcement learning algorithms where significant
research effort has been dedicated to devising a good curriculum to train these agent policies, engineer good representations of target belief states for agents to base their control policies on and ensure agents communicate their beliefs proactively to prevent
redundant search work.


