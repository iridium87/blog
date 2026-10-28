# Blog

A personal knowledge base and notes site built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/).

## About

This site is my external brain — a place to collect thoughts, learnings, and technical notes. Everything is written in Markdown and published automatically via GitHub Pages.

## How It Works

The workflow is intentionally simple:

1. **Write** a Markdown file in `_posts/`
2. **Commit** and push to GitHub
3. **Publish** — GitHub Pages builds and deploys automatically

Each post needs YAML front matter at the top:

```yaml
---
layout: post
title: "My Post Title"
date: 2026-10-28 16:00:00 +0100
categories: [notes, tech]
---
```

## Local Development

```bash
# Install Ruby and Bundler (one-time)
gem install bundler

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# View at http://localhost:4000
```

## GitHub Pages Setup

1. Create a repository named `blog` on GitHub
2. Push your site files to the `main` branch
3. Go to **Settings → Pages**
4. Select **"Deploy from branch"** → **`main`** → **`/root`**
5. Your site is live at `https://iridium87.github.io/blog/`

## Adding a New Post

```bash
# Create a new post file
touch _posts/YYYY-MM-DD-your-note.md

# Edit with your content, then:
git add .
git commit -m "Add post: Your Note Title"
git push
```

## Structure

```
/jekyll-blog
├── _config.yml        # Site configuration
├── _layouts/          # HTML templates
├── _posts/            # Your blog posts (Markdown)
├── assets/            # CSS, images, etc.
├── index.md           # Homepage
├── Gemfile            # Ruby dependencies
└── README.md          # This file
```

## License

This site is for personal use. Feel free to use the structure as a template for your own Jekyll blog.