---
layout: page
title: portfolio
permalink: /portfolio/
---

<div class="portfolio">
  {% for portfolio in site.portfolios %}
    <article class="portfolio {{ portfolio.tag }}">

      <h1><a href="{{ site.baseurl }}{{ portfolio.url }}">{{ portfolio.title }}</a></h1>

      <div class="entry">
        {{ portfolio.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ portfolio.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}