---
layout: default
title: blog
permalink: /blog/
bg-color: f9f9f9
fg-color: 111
---

<div class="posts">
  <h1>Posts</h1>

  {% for post in site.posts %}
    <article class="post {{ post.tag }}" style="{% if post.bg-color %}--bg-color: #{{ post.bg-color }}; {% endif %}{% if post.fg-color %}--fg-color: #{{ post.fg-color }}; {% endif %}">

      <a href="{{ site.baseurl }}{{ post.url }}" class="entry">{{ post.excerpt }}</a>

      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">{{ post.description }}</a>
      
      <div class="tag">{{ post.tag }}</div>

    </article>
  {% endfor %}