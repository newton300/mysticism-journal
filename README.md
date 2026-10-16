# Mysticism Journal

An elegant, responsive literary journal exploring Sufi literature, mysticism, and the wisdom of the heart. Built with Jekyll and designed for Cloudflare Pages.

## Local development

Requirements: Ruby and Bundler.

```sh
bundle install
bundle exec jekyll serve
```

Open the local URL printed by Jekyll (usually http://127.0.0.1:4000).

## Cloudflare Pages deployment

1. In Cloudflare, open **Workers & Pages** and create a Pages project connected to this GitHub repository.
2. Select the `main` branch.
3. Set **Build command** to `bundle exec jekyll build`.
4. Set **Build output directory** to `_site`.
5. Use a supported Ruby environment and install dependencies from `Gemfile`.
6. Deploy the project, then configure the custom domain in Cloudflare Pages when ready.

The repository contains the Jekyll source. A successful GitHub commit does not itself publish the website; the Pages project must be connected and deployed.

## Publishing an essay

Create a Markdown file in `_posts/` using this filename format:

`YYYY-MM-DD-short-title.md`

Add front matter at the top:

```yaml
---
title: "Your essay title"
date: 2026-10-16 09:00:00 +0000
category: Reflections
description: A concise description for search and sharing.
---
```

Write the essay below the front matter using Markdown.

## Site structure

- `index.html` — homepage
- `_layouts/` — shared and essay layouts
- `_posts/` — journal essays
- `essays/` — essay archive
- `traditions/` — writers and literary traditions
- `about.md` — editorial purpose
- `assets/css/style.css` — responsive visual design
