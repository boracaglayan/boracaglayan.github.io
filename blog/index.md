---
layout: default
title: Bora Caglayan
---

<div id="home">
  <h1>Articles</h1>
  <ul class="posts">
    {% for post in site.posts %}
    {% if post.categories contains 'eng' %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</div>
