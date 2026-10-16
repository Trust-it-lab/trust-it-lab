---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

{% comment %}
  HOW TO ADD A PROJECT: copy one <div class="research-card"> ... </div> block
  below and edit it. To add a picture, put the file in /images/research/ and
  uncomment the research-card__image block, changing the filename.
{% endcomment %}

<div class="research-card" markdown="1">

## Agentic AI for Microgrid Data Integrity

Microgrid controllers increasingly depend on data-driven analytics, but their decisions are only as good as the telemetry they receive. Our work identifies four interdependent factors that threaten operational data integrity in microgrids: data quality, packet loss, fault tolerance, and time synchronization. Because a disruption in one often shows up as a symptom in another, we explore agentic AI, in which coordinated, reasoning-capable AI agents detect, diagnose, and mitigate these issues jointly rather than in isolation. We also lay out a validation plan on a controller hardware-in-the-loop (CHIL) real-time testbed and identify open research directions in self-healing, cybersecurity, explainability, and multi-microgrid coordination. This work is a collaboration with Oak Ridge National Laboratory, the University of the Pacific, and the University of Tulsa.

<!--
<div class="research-card__image">
  <img src="{{ base_path }}/images/research/microgrid.png" alt="Agentic AI framework for microgrid data integrity">
</div>
-->

<p class="research-card__papers"><strong>Related paper:</strong>
<a href="https://www.researchgate.net/profile/Tapadhir-Das/publication/413939419_Agentic_AI_for_Microgrid_Operational_Data_Integrity_Key_Factors_Opportunities_Validation_Plan_and_Open_Research_Areas/links/6a999b72719cb76e27e08c27/Agentic-AI-for-Microgrid-Operational-Data-Integrity-Key-Factors-Opportunities-Validation-Plan-and-Open-Research-Areas.pdf">Agentic AI for Microgrid Operational Data Integrity: Key Factors, Opportunities, Validation Plan, and Open Research Areas</a> (IEEE Resilience Week 2026)</p>

</div>

<div class="research-card" markdown="1">

## Robustness of Deep Reinforcement Learning in Open Worlds

AI agents trained with deep reinforcement learning (DRL) often fail when the world changes in ways they never saw during training, such as wild animals crossing a city street during a pandemic or a traffic signal melting in a heat wave. These structural "novelties" can sharply degrade an agent's performance, yet the space of possible novelties grows combinatorially, so they cannot all be tested. We formalize novelty search as a budget-constrained search over a novelty tree and propose DeQNo, a deep Q-learning strategy that efficiently finds the novelties with the greatest negative impact on a black-box DRL agent. In experiments on the stochastic multi-agent game of Monopoly, DeQNo found more high-impact novelties than four baseline strategies, helping map the "safety envelope" of an agent before it is deployed. This research was supported in part by DARPA and the U.S. Air Force Research Laboratory.

<!--
<div class="research-card__image">
  <img src="{{ base_path }}/images/research/deqno.png" alt="DeQNo novelty search framework">
</div>
-->

<p class="research-card__papers"><strong>Related paper:</strong>
<a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10697140">A Q-Learning Novelty Search Strategy for Evaluating Robustness of Deep Reinforcement Learning in Open-World Environments</a> (IEEE Intelligent Systems, 2025)</p>

</div>
