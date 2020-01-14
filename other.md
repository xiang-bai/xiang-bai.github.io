---
layout: default
title: other
---

<div id="home">
    <h1>其他文章列表</h1>
    <ul class="posts">
        {% for post in site.categories.other %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
        {% endfor %}
    </ul>
</div>
