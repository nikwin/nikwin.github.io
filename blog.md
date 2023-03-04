---
layout: base
title: Blog
---

# Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      {{ post.desc }}
    </li>
  {% endfor %}
</ul>