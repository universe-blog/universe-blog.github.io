# Universe Blog

Source for **Universe Blog**, built with [Jekyll](https://jekyllrb.com) and
published with GitHub Pages.

🌐 Live site: https://universe-blog.github.io/

## How it works

You write posts in Markdown; GitHub Pages builds the HTML automatically on every
push to the deployed branch — no local build or GitHub Actions workflow needed.
The RSS/Atom feed (`/feed.xml`) and `sitemap.xml` are generated automatically by
the `jekyll-feed` and `jekyll-sitemap` plugins.

## Add a new post

Create a file in `_posts/` named `YYYY-MM-DD-title.md`:

```markdown
---
layout: post
title: "My Post Title"
date: 2026-10-31
author: Eze Ahuna
---

Your post content goes here, in Markdown.
```

Commit and push. The post appears at
`https://universe-blog.github.io/YYYY/MM/DD/title/`.

## Add a static page

Create e.g. `contact.md` with front matter `layout: page` and a `permalink`,
then push.

## Preview locally (optional)

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Layout

```
_config.yml      site settings (title, URL, theme, plugins)
index.md         home page (lists posts)
about.md         example static page
_posts/          blog posts (Markdown)
media/           images used by posts
```

The theme is `minima` (GitHub Pages' default). To restyle, change `theme:` in
`_config.yml` or override files under `_layouts/`, `_includes/`, and `assets/`.
