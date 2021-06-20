---
title: cloud
layout: default
---
<ul>
  {% assign posts = site.posts | where_exp:"page","page.categories contains 'cloud'" %}
  {% for post in posts %}
      <h6>{{ post.date | date: "%Y-%m-%d" }}</h6>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
  {% endfor %}
</ul>