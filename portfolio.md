---
layout: default
title: portfolio
permalink: /portfolio/
bg-color: 111
fg-color: fff
---

<div class="portfolio">
  <h1>Portfolio</h1>

  {% for portfolio in site.portfolios %}
    <article  class="portfolio {{ portfolio.tag }}" style="{% if portfolio.bg-color %}--bg-color: #{{ portfolio.bg-color }}; {% endif %}{% if portfolio.fg-color %}--fg-color: #{{ portfolio.fg-color }}; {% endif %}">

      <a href="{{ site.baseurl }}{{ portfolio.url }}" class="entry">{{ portfolio.excerpt }}</a>

      <h3><a href="{{ site.baseurl }}{{ portfolio.url }}">{{ portfolio.title }}</a></h3>

      <a href="{{ site.baseurl }}{{ portfolio.url }}" class="read-more">{{ portfolio.description }}</a>
      
      <div class="tag">{{ portfolio.tag }}</div>
    </article>
  {% endfor %}