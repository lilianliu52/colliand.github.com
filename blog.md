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

<!-- <div class="home">

  <h1 class="page-heading">Lectures</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%A, %Y-%m-%d" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div> -->


<div id="home">
  <h1>Blog Posts</h1>
  <ul class="posts">
    {% for post in site.posts %}
      <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li> -->
       <li><span>{{ post.date | date: "%Y-%m-%d" }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>
 
<!-- 
<div id="home">
  <h1>Math 217: Multivariable and Vector Calculus</h1>
  <h2>Lectures</h2>
  <ul class="posts">
    {% for post in site.posts %}
      <li><span>{{ post.date | date: "%Y-%m-%d" }}</span> &raquo; <a href="{{site.baseurl}}{{ post.url }}">{{ post.title }} &raquo;
               {% for tag in post.tags %}   
  <a href="{{site.baseurl}}/tags#{{ tag }}-ref" class='list-group-item'>
       {{ tag }} <span class='badge'>{{ site.tags[tag].size }}</span>
      </a>
     {% endfor %} 
        
      </a></li> 
    {% endfor %}
  </ul>
</div> -->