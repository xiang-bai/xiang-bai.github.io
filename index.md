---
layout: default
title: 13AI
---

<div id="home">
  <h1>个人文章列表</h1>
  <ul class="posts">
    {% for post in site.posts %}
    {% if post.categories == math %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
    {% endfor %}
  </ul>

  <h1>好文推荐</h1>
  <ul class="posts">
    <li><span>27 Mar 2019</span> &raquo; <a href="https://www.quantamagazine.org/math-proof-finds-all-change-is-mix-of-order-and-randomness-20190327/">Proof Finds That All Change Is a Mix of Order and Randomness</a></li>
    <li><span>29 Mar 2019</span> &raquo; <a href="http://www.markdown.cn/"> Markdown 语法说明</a></li> 
    <li><span>01 May 2019</span> &raquo; <a href="https://inkscape.org/zh/learn/tutorials/"> Inkscape 教程</a></li> 
  
  </ul>

</div>
