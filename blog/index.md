---
layout: default
title: Блог
permalink: /blog/
---

# Блог

Здесь публикуются мои статьи и размышления.

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) <small>{{ post.date | date: "%d.%m.%Y" }}</small>
{% endfor %}