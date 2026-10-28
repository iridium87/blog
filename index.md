---
layout: default
title: Home
---

# Welcome to My Notes

Hello! This is my personal knowledge base and notes site, built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/).

## How it works

This site is incredibly simple: I write notes as Markdown files in the `_posts/` directory, and Jekyll automatically turns them into a publishable blog. Every time I push to GitHub, GitHub Pages rebuilds and deploys the site.

## Recent Posts

{% for post in site.posts %}
<h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
<p>{{ post.excerpt }}</p>
<small>{{ post.date | date: "%B %d, %Y" }}</small>
{% endfor %}

## About Me

I'm a developer and tinkerer interested in AI, games, and systems programming. You can find me on GitHub at [@yourusername](https://github.com/yourusername).