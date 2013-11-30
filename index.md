---
layout: default
title: harx
---

{% for post in site.posts %}
	<div class="jumbotron">
		<h3><a href="{{ post.url }}">{{ post.title }}</a>  <small>{{post.date|date_to_string}}</small></h3>
	</div>	
{% endfor %}

<!-- FOOTER  -->
<div id="footer_wrap" class="outer">
	<footer class="inner">
		<p>Published with <a href="http://pages.github.com">GitHub Pages</a></p>
		<a id="forkme_banner" href="https://github.com/Harx">View on GitHub</a>
	</footer>
</div>
