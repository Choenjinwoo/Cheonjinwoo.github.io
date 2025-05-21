---
layout: default
title: "History"
permalink: /categories/history/
---

<h1>Category: History</h1>

<ul>
  {% for post in site.posts %}
    {% if post.category == "history" %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
