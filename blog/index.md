---
layout: default
title: Блог
permalink: /blog/
---

# 📰 Блог

<div class="blog-list">
  {% for post in site.posts %}
    <a class="blog-link" href="{{ site.baseurl }}{{ post.url }}">
      <div class="blog-card">
        <div class="blog-title">{{ post.title }}</div>
        <div class="blog-date">{{ post.date | date: "%d.%m.%Y" }}</div>
      </div>
    </a>
  {% endfor %}
</div>