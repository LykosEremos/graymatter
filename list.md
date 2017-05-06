---
layout: page
title: 文章列表
permalink: /list/
---
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <div class="post-list-title">
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </div >
      </li>
    {% endfor %}
  </ul>