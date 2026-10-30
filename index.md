---
layout: default
title: Home
---

<h>Homepage</h>
<p>This is my personal website. Opinions are my own.</p>
<p>I'm a developer and tinkerer interested in AI, games, and systems programming. You can find me on GitHub at <a href="https://github.com/{{ site.github }}">@{{ site.github }}</a>.</p>
<p><a href="/about.html">Read more about me →</a></p>

<h>Articles</h>
<p style="text-align: left; margin-bottom: 1ch;">
{% for post in site.posts reversed %}
  {{ post.date | date: "%d/%m/%Y" }}: <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><br>
{% endfor %}
</p>
