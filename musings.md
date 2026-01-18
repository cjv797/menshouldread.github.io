---
layout: page
title: Musings
permalink: /musings/
---

<ul>
  {% for post in site.categories.musings %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      — {{ post.date | date: "%b %d, %Y" }}
    </li>
  {% endfor %}
</ul>
