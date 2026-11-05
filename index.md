---
layout: default
title: Home
---

<h>Homepage</h>
<p>This is my personal website. Opinions are my own.</p>
<p>Gamedev, LLMs, physical AI. I write about what I'm tinkering with when I have something worth saying. You can find me on GitHub at <a href="https://github.com/{{ site.github }}">@{{ site.github }}</a>.</p>
<p><a href="/about.html">Read more about me →</a></p>

<h>Articles</h>
<p style="text-align: left; margin-bottom: 1ch;">
{% for post in site.posts reversed %}
  {{ post.date | date: "%d/%m/%Y" }}: <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><br>
{% endfor %}
</p>
