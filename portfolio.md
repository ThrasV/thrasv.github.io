---
layout: default
title: portfolio
permalink: /portfolio/
---

<div class="portfolio">
  {% for portfolio in site.portfolios %}
    <article class="portfolio {{ portfolio.tag }}" style="{% if portfolio.bg-color %}--bg-color: #{{ portfolio.bg-color }}; {% endif %}{% if portfolio.fg-color %}--fg-color: #{{ portfolio.fg-color }}; {% endif %}">

      <h1><a href="{{ site.baseurl }}{{ portfolio.url }}">{{ portfolio.title }}</a></h1>

      <div class="entry">
        {{ portfolio.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ portfolio.url }}" class="read-more">Read More</a>
      
      <div class="tag">{{ portfolio.tag }}</div>
    </article>
  {% endfor %}