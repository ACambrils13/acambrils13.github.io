---
layout: page
title: Reseñas
permalink: /resenas/
description: Reseñas, comentarios y apuntes de lectura.
---

# Reseñas y apuntes

Aquí reuniré comentarios más personales: qué me ha parecido un libro, qué funciona, qué me ha sorprendido y a quién se lo recomendaría.

Las entradas nuevas aparecerán automáticamente debajo:

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%d.%m.%Y" }}</span>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      {% if post.excerpt %}<p>{{ post.excerpt | strip_html }}</p>{% endif %}
    </li>
  {% endfor %}
</ul>

