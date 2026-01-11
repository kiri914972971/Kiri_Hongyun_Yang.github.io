---
layout: archive
title: "Projects"
permalink: /portfolio/
author_profile: true
---

Here are some selected projects showcasing my work in data analysis, product thinking, and business insights.

{% assign projects = site.portfolio | sort: "date" | reverse %}

{% assign projects = site.portfolio | sort: "date" | reverse %}

<div class="grid__wrapper">
  {% for p in projects %}
    <div class="grid__item">
      <article class="archive__item">
        <h2 class="archive__item-title">
          <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
        </h2>

        {% if p.excerpt %}
          <p class="archive__item-excerpt">{{ p.excerpt }}</p>
        {% endif %}

        <p><a class="btn btn--primary" href="{{ p.url | relative_url }}">View project →</a></p>
      </article>
    </div>
  {% endfor %}
</div>
