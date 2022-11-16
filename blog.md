---
layout: page
title: Blog
---

<h1>Latest Posts</h1>
<h2>(_layout: page 비교용 사이트)</h2>
<ul>
  {% for post in site.posts %}
  <li>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </li>
  {% endfor %}
</ul>

<a href="{{ site.baseurl }}{{ post.url }}" class="read-more">
        {{post.excerpt | truncate: 50, '...' }}</a>
