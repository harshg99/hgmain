---
layout: page
title: Multi-agent Foraging
description: Multi agent reinforcement learning for foraging agents to accumulate and store resources from the environment
importance: 2
category: Classes
---


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/quad_control_gcrl/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>



We focus on the multi agent foraging task, where a group of agents collect resources and deposit them at a central depo in a collaborative manner.
Existing decentralised solutions to foraging problem are often rule based and don’t take into account multiple objectives of exploration and
exploitation for foraging, or resource constraints in agents. Our paper’s contributions are to apply a reinforcement learning solution to the
multi agent foraging problem, which gives us the advantage of making a NP-hard foraging problem computationally feasible,decentralised and scalable to any number of agents under resource constraints.

Agents would be deployed in an environment with food and water as shown in Figure 1 and each agent will collect and deposit resources while
consuming a few resources to survive. This paper aims to investigate the emergence of behaviour that balances between exploitation of resources
for individual survival and the team objective of depositing resources at a Depo through Reinforcement Learning. Learning for Multi agent systems
can be difficult to stabilise due to non-stationarity[4] in the environment and as such we apply newer techniques in Reinforcement Learning, 
specifically Proximal Policy Optimisation (PPO) to train a policy. We design and compare learned policies over two reward structures for the problem.
