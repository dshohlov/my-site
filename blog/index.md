---
layout: default
title: Блог
permalink: /blog/
---

# 📰 Блог

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) <small>{{ post.date | date: "%d.%m.%Y" }}</small>
{% endfor %}