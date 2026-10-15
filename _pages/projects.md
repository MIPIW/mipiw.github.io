---
layout: page
title: research
permalink: /projects/
description: Research directions. Status is stated for each; unpublished work is exploratory.
nav: true
nav_order: 3
display_categories: [interpretability, evaluation, linguistics]
horizontal: false
---

<div class="projects">
{% assign sorted = site.projects | sort: "importance" %}
{% for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {% assign items = sorted | where: "category", category %}
  <div class="row row-cols-1 row-cols-md-2">
  {% for project in items %}
    {% include projects.liquid %}
  {% endfor %}
  </div>
{% endfor %}
</div>
