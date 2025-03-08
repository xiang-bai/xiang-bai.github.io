---
layout: default
title: math
---

<div id="home">
    <h1>数学文章列表</h1>
    <ul class="posts">
        {% for post in site.categories.math %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
        {% endfor %}
    </ul>
</div>
