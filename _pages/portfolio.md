---
layout: archive
title: "Projects"
permalink: /portfolio/
collection: portfolio
entries_layout: list
author_profile: true
---

Here are some selected projects showcasing my work in data analysis, product thinking, and business insights.

{% assign projects = site.portfolio | sort: "date" | reverse %}

<div class="grid__wrapper">
  {% for post in projects %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
