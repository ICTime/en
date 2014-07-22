---
layout: page
title: Random Walk 
tagline: A Timing Engineer's Work and Imagnation 
---
{% include JB/setup %}

<!---
-->
<img src="http://ictime.github.com/image/local.jpg"  width="120" height="150" title="ICTimer" align="right" />

Welcome to ICTime  

My Name is YU Bing, and I am an ASIC Physical Design Engineer at [NVIDIA](http://www.nvidia.com/page/home.html). Currently I am focusing on the Static Timing Analysis, include but not limited to constraint and timing closure of cutting edge GPU/Mobile chips.  

I love engineering as a profession that providing better solutions for hard problems. I also have passion on [Market Timing](http://en.wikipedia.org/wiki/Market_timing)  

### Latest Posts 

<ul class="posts">
  {% for post in site.posts limit:5 %}
    <li><span>{{ post.date | date_to_utc | date: '%Y-%m-%d' }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

### 中文页面
中文读者请移步[中文页面](http://ictime.github.com/)
