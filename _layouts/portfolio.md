---
layout: default
---

<article class="portfolio-entry {{ page.tag }}">
  <h1>{{ page.title }}</h1>
  
  <div class="tag">{{ page.tag }}</div>

  <div class="entry">
    {{ content }}
  </div>

  <div class="date">
    Written on {{ page.date | date: "%B %e, %Y" }}
  </div>
</article>
