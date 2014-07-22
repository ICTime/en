---
layout: page
title: Random Walk 
tagline: A Timing Engineer's Work and Imagnation 
---
{% include JB/setup %}

<!---
-->
<img src="http://ictime.github.com/image/local.jpg"  width="120" height="150" title="ICTimer" align="right" />

Welcome to ICTime, this pages is only a place holder for english version of blog. 

### Latest Posts 

<ul class="posts">
  {% for post in site.posts limit:5 %}
    <li><span>{{ post.date | date_to_utc | date: '%Y-%m-%d' }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

### 中文页面
中文读者请移步[中文页面](http://ictime.github.com/cn)
