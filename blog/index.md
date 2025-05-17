---
layout: default
title: Блог
permalink: /blog/
---

# Блог

<div class="blog-list">
  {% for post in site.posts %}
    <a class="blog-link" href="{{ site.baseurl }}{{ post.url }}">
      <div class="blog-card{% if post.title contains "Stepik" %} blog-card-stepik{% endif %}">
        <div class="blog-title">
          {% if post.title contains "Stepik" %}
            <span class="blog-tag-stepik">Stepik</span>
          {% endif %}
          {{ post.title }}
        </div>
        <div class="blog-date">{{ post.date | date: "%d.%m.%Y" }}</div>
        {% if post.description %}
          <div class="blog-desc">{{ post.description }}</div>
        {% endif %}
      </div>
    </a>
  {% endfor %}
</div>