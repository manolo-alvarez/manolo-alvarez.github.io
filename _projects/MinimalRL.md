---
layout: page
title: Minimal Policy for Locomotion
description: TBU
img: TBU
importance: 1
category: academic
#related_publications: 
---
<div class="caption">
    <b>Abstract</b>
</div>
In this work, my teammates and I investigate the minimal propioceptive pipeline for stable locomotion of a toy humanoid. Using PPO, we establish a baseline walking policy for the Zbot toy humanoid and conduct a feature importance analysis on the policy to screen out nonessential sensory inputs. We also explore alternative learning architectures inspired by Versatile Motion Priors (VMP) and Temporal Difference Model-Predictive Control (TDMPC) hypothesizing that their more explicit modeling of the environment could make up for the reduced set of observations. We are able to match the quantitative and qualitative performance of our baseline with a 10% drop in observations guided by our feature analysis but fail to produce comparable policies via VMP and TDMPC. Our results highlight the challenges of reducing input dimensionality and the trade-offs in model-based and prior-driven methods. 

<div class="image">
{% include figure.html path="TBU" title="Method" class="img-fluid rounded z-depth-1" %}
</div>​
