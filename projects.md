---
layout: page
title: Projects
permalink: projects/
---

Things I do, including research, engineering projects, and miscellaneous interests.


## Research

Research publications for AI Agent, RL, Causality and Interpretability.

<div class="project-spacer-small"></div>

<div class="l-page project-grid">
    {% for project in site.categories.papers %}
    {% include project.html project=project %}
    {% endfor %}
</div>

<div class="project-spacer"></div>

## Engineering

Innovative AI systems and products I've developed and deployed at scale.

<div class="project-spacer-small"></div>

<div class="l-page project-grid">
    {% assign sortedArticles = site.data.articles | where: "featured", true %}
    {% assign ia = site.categories.papers | where:"permalink", "papers/interactive-articles" %}

    {% for feature in sortedArticles %}
        {% include feature.html feature=feature %}
    {% endfor %}

    {% assign feature = ia[0] %}
    {% include feature.html feature=feature %}
</div>
