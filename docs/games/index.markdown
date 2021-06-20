---
title: games
layout: default
---
<ul>
  {% assign posts = site.posts | where_exp:"page","page.categories contains 'games'" %}
  {% for post in posts %}
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
  {% endfor %}
</ul>