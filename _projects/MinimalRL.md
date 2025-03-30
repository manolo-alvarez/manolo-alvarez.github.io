---
layout: page
title: Minimal proprioception
description: Explored the minimal proprioceptive pipeline for stable locomotion of a toy humanoid
img: assets/img/zbot.png
importance: 1
category: academic
#related_publications: 
---
<div class="caption">
    <b>Overview</b>
</div>
In this work, my teammates and I investigated the minimal proprioceptive pipeline for stable locomotion of a toy humanoid. Using PPO, we established a baseline walking policy for the Zbot toy humanoid and conducted a feature importance analysis on the policy to screen out nonessential sensory inputs. We also explored alternative learning architectures inspired by Versatile Motion Priors (VMP) and Temporal Difference Model-Predictive Control (TDMPC) hypothesizing that their more explicit modeling of the environment could make up for the reduced set of observations. We were able to match the quantitative and qualitative performance of our baseline with a 10% drop in observations guided by our feature analysis but failed to produce comparable policies via VMP and TDMPC. Our results highlighted the challenges of reducing input dimensionality and the trade-offs in model-based and prior-driven methods. 

I was responsible for the feature analysis, re-training the baseline with the new URDF, adapting TDMPC, sim transfer to kos-sim, and repo maintainance.

<div class="caption">Team Picture</div>
<div class="image">
{% include figure.html path="assets/img/minimalRL_team.jpeg" title="Team" class="img-fluid rounded z-depth-1" %}
</div>

<div class="caption">Minimal Policy on Hardware</div>
<video width="100%" height="auto" controls>
  <source src="../../assets/video/minimalRL.mp4" type="video/mp4">
</video>

<div class="caption">Full Paper</div>
<iframe src="../../assets/pdf/minimalRL.pdf" style="width: 100%; height: 100vh"></iframe>
