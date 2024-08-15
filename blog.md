---
layout: default
title: Blog
permalink: /blog/
---
<h1>{{ page.title }}</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
      <!--
      <p>{{ post.excerpt }}</p>
      -->
    </li>
  {% endfor %}
</ul>
