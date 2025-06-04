---
layout: default
title: "history"
permalink: /categories/history/
---

<!-- Section: Archive - Category: history -->
<section class="section section-inner m-archive">
  <div class="container">

    <div class="m-titles align-center">
      <h1 class="m-title">Category: {{ page.title | capitalize }}</h1>
      <div class="m-subtitle">포스트 목록</div>
    </div>

    <div class="articles-container">
      {% for post in site.posts %}
        {% if post.categories contains page.title %}
          <div class="archive-item">
            <h3>
              <a href="{{ post.url }}">{{ post.title }}</a>
            </h3>
            <p class="post-date">{{ post.date | date: "%Y-%m-%d" }}</p>
            <p>{{ post.excerpt }}</p>
            <a href="{{ post.url }}" class="lnk">Read More →</a>
          </div>
        {% endif %}
      {% endfor %}
    </div>

  </div>
</section>
