---
layout: default
title: portfolio
permalink: /portfolio/
---

<div class="portfolio">
  {% for portfolio in site.portfolios %}
    <article class="portfolio {{ portfolio.tag }}" style="{% if portfolio.bg-color %}--bg-color: #{{ portfolio.bg-color }}; {% endif %}{% if portfolio.fg-color %}--fg-color: #{{ portfolio.fg-color }}; {% endif %}">

      <div class="entry">{{ portfolio.excerpt }}</div>

      <h2><a href="{{ site.baseurl }}{{ portfolio.url }}">{{ portfolio.title }}</a></h2>

      <a href="{{ site.baseurl }}{{ portfolio.url }}" class="read-more">{{ portfolio.description }}</a>
      
      <div class="tag">{{ portfolio.tag }}</div>
    </article>
  {% endfor %}