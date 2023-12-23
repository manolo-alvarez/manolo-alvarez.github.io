---
layout: page
title: Trip Weaver
description: Tuning a foundational LLM to formulate comprehensive travel itineraries within the bounds of consumer hardware.
img: assets/img/TripWeaver/TripWeaver.png
importance: 1
category: academic
#related_publications: einstein1956investigations
---
<div class="caption">
    <b>Abstract</b>
</div>
Travel is a fun, enriching experience that often succumbs to the burdensome weight of intricate planning and intractable financial estimates. This project attempts to relief that stress by creating an artificially intelligent agent capable of formulating comprehensive travel itineraries with cost approximations, tailored to individual preferences, and within the bounds of consumer hardware. The agent, a large language model (LLM), is tuned via Quantized Low-Rank Adapters (QLoRA), maximum-likelihood training on expert itineraries (SFT), and implicit reward models through Direct Preference Optimization (DPO). In evaluation, the 7 billion quantized parameter SFT and DPO models improve significantly over the baseline with the SFT model approximating the quantitative and qualitative performance of GPT-3.5.

<div class="caption">
    <b>Method</b>
    <div class="image">
    {% include figure.html path="assets/img/TripWeaver/TripWeaver.png" title="Method" class="img-fluid rounded z-depth-1" %}
    </div>​
</div>

<div class="caption">
    <b>Example Completions</b>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/TripWeaver/itinerary_GPT-3.5-Turbo-1106_Austin_temp-1.0_top-p-1.0.png" title="GPT-3.5-Turbo-1106" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            GPT-3.5-Turbo-1106
        </div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/TripWeaver/itinerary_llama2-7b_Austin_temp-1.0_top-p-1.0_1.png" title="Baseline (Vanilla Quantized 7b Llama-2)" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Baseline (Vanilla Quantized 7b Llama-2)
        </div>
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/TripWeaver/itinerary_llama2-7b_SFT_Austin_temp-1.0_top-p-1.0_1.png" title="SFT" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            SFT
        </div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/TripWeaver/itinerary_llama2-7b_DPO_Austin_temp-1.0_top-p-1.0_new.png" title="DPO" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            DPO
        </div>
    </div>
</div>

