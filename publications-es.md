---
layout: default
title: Resúmenes en Español
---

# Resúmenes en Español

<p>Aquí se encuentran los resúmenes de mis publicaciones científicas en mi lengua natal. Por una Ciencia global multilingüe, inclusiva y diversa.</p>

<div class="feature-grid">
  {% for post in site.posts %}
    <div class="card">
      {% if post.image %}
        <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" style="width:100%; height:auto; border-radius:4px;">
      {% endif %}
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url | relative_url }}" class="btn btn-outline">Leer más</a>
    </div>
  {% endfor %}
</div>
