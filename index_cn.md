---
layout: default
title: Bai's homepage
---

<div id="home">
  <p><img src="/bai.png" width="90" style="float:right"><b> Xiang Bai</b><br>某高校教师<br>某学院<br>Beijing, P.R. China
<br>Email: ottiou.bai@gmail.com <br>Ocrid: </p>

  <h1> 研究兴趣 </h1>
  <h1> 履历 </h1>
  <h1> 笔记列表 </h1>
  <ul class="posts">
    {% for cat in site.categories %}
      {% if cat[0] == "math" %}
        <h1> 数学文章列表 </h1>
        {% for post in cat[1] %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
      {% endif %}
      {% if cat[0] == "AI" %}
        <h1> {{ cat[0] }}文章列表 </h1>
        {% for post in cat[1] %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
      {% endif %}
      {% if cat[0] == "other" %}
        <h1> 其他文章列表 </h1>
        {% for post in cat[1] %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
      {% endif %}
    {% endfor %}
  </ul>

  <h1>相关推荐</h1>
  <ul class="posts">
    <!-- <li><span>29 Mar 2019</span> &raquo; <a href="http://www.markdown.cn/"> Markdown 语法说明</a></li>  -->
    <li><span>01 May 2019</span> &raquo; <a href="https://inkscape.org/zh/learn/tutorials/"> Inkscape 教程</a></li> 
    <li><span>01 May 2019</span> &raquo; <a href="https://jekyllrb.com/tutorials/navigation/#scenario-8-retrieving-items-based-on-front-matter-properties"> jekyll 教程</a></li> 
    <li><span>01 May 2020</span> &raquo; <a href="http://www.texample.net/tikz/"> tikz 官网</a></li> 
  
  </ul>

</div>

