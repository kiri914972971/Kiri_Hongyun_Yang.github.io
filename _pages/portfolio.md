---
layout: archive
title: "Projects"
permalink: /portfolio/
collection: portfolio
entries_layout: list
author_profile: true
author: academicpages
---

以下是一些精选项目，展示了我在数据分析、产品思维和商业洞察方面的工作。

{% assign projects = site.portfolio | sort: "date" | reverse %}

<div class="portfolio-list">
  {% for post in projects %}
    <article class="portfolio-item">
      {% if post.header.teaser %}
        <a class="portfolio-item__teaser" href="{{ post.url | relative_url }}">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}">
        </a>
      {% endif %}

      <div class="portfolio-item__body">
        <h2 class="archive__item-title">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h2>

        <p class="page__date">
          <strong><i class="far fa-calendar-alt" aria-hidden="true"></i> Published:</strong>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
        </p>

        {% if post.excerpt %}
          <p class="archive__item-excerpt">{{ post.excerpt }}</p>
        {% endif %}
      </div>
    </article>
  {% endfor %}
</div>
