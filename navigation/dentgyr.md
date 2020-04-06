---
layout: page
landing: dentgyr
title: 齿状回
show: hide
permalink: /dentgyr/
---
<div style="size=0.8em;color:#9b9b9b; margin-bottom:2em;">「灰质」上的所有文章，分类视图. 点此回到<a href="{{site.baseurl}}/hippocampus">海马体</a></div>
{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{site.baseurl}}/{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
