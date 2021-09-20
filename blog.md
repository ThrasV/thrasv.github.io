---
layout: default
title: blog
permalink: /blog/
bg-color: f9f9f9
fg-color: 111
---

<div class="posts">
  {% for post in site.posts %}
    <article class="post {{ post.tag }}">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}