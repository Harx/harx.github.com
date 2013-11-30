---
layout: default
title: harx's blog
---

<h2>{{ page.title }}</h2>
<h4>{{post.title}}</h4>

<p>最新文章56</p>
<ul>
{% for post in site.posts %}
<li>{{ post.date | date_to_string }} <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
