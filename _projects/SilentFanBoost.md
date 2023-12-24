---
layout: page
title: Silent Fan Boost
description: Learning system fan and ambient noise combinations audible to PC users
img: assets/img/SilentFanBoost.png
importance: 2
category: academic
#related_publications:
---
<u>Note</u>: scroll to the bottom of this page for the full paper.

<div class="caption">
    <b>Introduction</b>
</div>
The goal of this project was to create a model that can learn the influence fan speeds have on an environment's noise and to identify and ignore spontaneous sound.

In practice, a software would feed the model a short recording from the system microphone and the current and future fan speeds to predict the prominence ratio of each of the fan's harmonics. That would be one iteration. The software would run the model for every possible "future" fan speed and use that to find and change to the highest predicted inaudible fan speed. In other words, the model would predict how audible every other fan speed (RPM) the system could change to would be. See illustration below.
<div class="image">
{% include figure.html path="assets/img/SilentFanBoostGoal.png" title="Method" class="img-fluid rounded z-depth-1" %}
</div>

<div class="caption">
    <b>Motivation</b>
</div>
Operating power in PC's is a function of thermal and acoustic constraints, and the higher it is, the faster a system will run. Most Original Equipment Manufacturer's (OEM's) set these as static constraints defined by user-configurable operating modes like "Cool," "Quiet," "Balanced," and "Performance," modes.

Static thermal and acoustic operating modes over-constrain system power levels in environments where such parameters have a negligible effect on customer experience. Sone (noise) limits are intended to prevent users from experiencing uncomfortable fan noise in the most "common" environment but the distribution of noise-level across environments is a wide one and this static limit does not take opportunistic advantage of environmental factors that boost system performance at the expense of unnoticeable fan noise to the customer.
 
<div class="caption">Full Paper</div>
<div class="center">
    <embed src="../../assets/pdf/SilentFanBoost.pdf" width="100%" height="900px" />
</div>

