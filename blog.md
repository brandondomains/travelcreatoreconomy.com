---
layout: page
title: Blog
eyebrow: Analysis archive
description: Essays and practical analysis on monetization, travel creator partnerships, audience growth, platform strategy, and creator economics.
permalink: /blog/
---
<div class="post-list">
{% for post in site.posts %}
  <article class="post-card">
    <p class="meta">{{ post.date | date: "%B %-d, %Y" }}{% if post.category %} · {{ post.category }}{% endif %}</p>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.description }}</p>
  </article>
{% endfor %}
</div>
