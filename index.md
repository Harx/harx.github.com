---
layout: default
title: harx's blog
---

{% for post in site.posts %}
	<div class="jumbotron">
		<h3><a href="{{ post.url }}">{{ post.title }}</a>  <small>{{post.date|date_to_string}}</small></h3>
	</div>	
{% endfor %}
