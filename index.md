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

I am a big believer that an engineer can always fix broken things, and develop better solutions for work or personal issues. 
And I love the rule “Keep It Simple”. Github Pages serves me right in the geek way of blogging, documentation and scripting (Hardware engineer don’t coding)  

I also send some time now and then practicing [Market Timing](http://en.wikipedia.org/wiki/Market_timing), I did *NOT* profit from my speculation yet, This is just another area that I applying my academic and engineering skills. 


### Latest Posts 

<ul class="posts">
  {% for post in site.posts limit:5 %}
    <li><span>{{ post.date | date_to_utc | date: '%Y-%m-%d' }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

### 中文页面
中文读者请移步[中文页面](http://ictime.github.com/)
