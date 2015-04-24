---
author: James Colliander
title: Blog
excerpt: James Colliander's Blog
layout: default
permalink: /blog/
published: true
id: /blog
icons: true
---

<div id="home">
  <h1>Blog Posts</h1>
  <ul class="posts">
    {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>