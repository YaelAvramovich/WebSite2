---
date: 2024-02-10
title: Getting Started with MkDocs Material
description: Learn how to set up a beautiful, feature-rich documentation site using MkDocs and the Material theme.
categories:
  - Tutorials
tags:
  - mkdocs
  - material
  - static-sites
---

# Getting Started with MkDocs Material 📚

[MkDocs Material](https://squidfunk.github.io/mkdocs-material/) is one of the best ways to
build a fast, beautiful, and accessible website from Markdown files. In this post, I'll walk
you through a minimal setup and highlight some of the most useful features.

<!-- more -->

## Installation

You'll need Python 3.8 or higher. Install MkDocs and the Material theme with:

```bash
pip install mkdocs-material
```

## Basic configuration

Create a `mkdocs.yml` file in your project root:

```yaml
site_name: My Site
theme:
  name: material
  palette:
    - scheme: default
      toggle:
        icon: material/brightness-7
        name: Switch to dark mode
    - scheme: slate
      toggle:
        icon: material/brightness-4
        name: Switch to light mode
```

## Adding pages

All your content lives inside the `docs/` folder. The `nav:` key in `mkdocs.yml` controls
what appears in the navigation:

```yaml
nav:
  - Home: index.md
  - Blog: blog/index.md
  - Contact: contact.md
```

## Enabling the blog

Material's built-in blog plugin makes it easy to manage posts:

```yaml
plugins:
  - search
  - blog
```

Place posts inside `docs/blog/posts/` with a date in the front matter, and they'll be
automatically indexed, archived, and categorised.

## Deploying to GitHub Pages

Add this GitHub Actions workflow (`.github/workflows/deploy.yml`) and push to `main` — your
site will be live at `https://<username>.github.io/<repo>/` within minutes:

```yaml
on:
  push:
    branches: [main]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-python@v5
        with:
          python-version: '3.x'
      - run: pip install mkdocs-material
      - run: mkdocs gh-deploy --force
```

---

That's the essentials! The [official documentation](https://squidfunk.github.io/mkdocs-material/)
covers every feature in depth — it's worth bookmarking.
