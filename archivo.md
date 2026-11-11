---
layout: page
title: Archivo
permalink: /archivo/
description: Todas las entradas de esta bitácora, ordenadas por fecha.
---

# Archivo

Un índice cronológico de las entradas publicadas.

{% assign current_year = "" %}
{% for post in site.posts %}
  {% assign post_year = post.date | date: "%Y" %}
  {% if post_year != current_year %}
    {% unless forloop.first %}</ul>{% endunless %}
    <h2>{{ post_year }}</h2>
    <ul class="archive-list">
    {% assign current_year = post_year %}
  {% endif %}
  <li><time>{{ post.date | date: "%d %b" }}</time> <a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
  {% if forloop.last %}</ul>{% endif %}
{% endfor %}
