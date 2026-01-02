---
layout: page
title: Blog
permalink: /blog/
---
<ul class="postlist">
  {% for post in site.posts %}
    <li class="postlist__item">
      <a class="postlist__title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <div class="postlist__meta">{{ post.date | date: "%b %-d, %Y" }}</div>
      {% if post.excerpt %}<div class="postlist__excerpt">{{ post.excerpt }}</div>{% endif %}
    </li>
  {% endfor %}
</ul>
