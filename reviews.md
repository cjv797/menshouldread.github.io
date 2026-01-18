---
layout: page
title: Reviews
permalink: /reviews/
---

<ul>
  {% for post in site.posts %}
    {% unless post.categories contains "musings" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        — {{ post.date | date: "%b %d, %Y" }}
        {% if post.media %} ({{ post.media }}) {% endif %}
        {% if post.rating %} — Rating: {{ post.rating }}/5 {% endif %}
      </li>
    {% endunless %}
  {% endfor %}
</ul>
