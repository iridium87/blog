---
layout: default
title: Posts
---

# All Posts

{% for post in site.posts %}
<h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
<p>{{ post.excerpt }}</p>
<small>{{ post.date | date: "%B %d, %Y" }}</small>
{% endfor %}
