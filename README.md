# Personal academic website

A minimal Jekyll site with three pages: About, Blog, Papers. GitHub Pages builds it automatically, so no CI setup is needed.

Live at https://parksean7.github.io/

## Deploy

GitHub Pages builds the `main` branch automatically. Every push to `main` updates the site within a minute or two.

## Customize

| What | Where |
|---|---|
| Name, role, email, social links | `_config.yml` (`author:` block) and `url` |
| Introduction text | `index.md` |
| Profile photo | Replace `assets/img/profile.svg` (or add `profile.jpg` and update the path in `index.md`) |
| Colors and fonts | Variables at the top of `assets/css/style.css` |

## Write a blog post

Add a file to `_posts/` named `YYYY-MM-DD-some-title.md`:

```markdown
---
layout: post
title: "My Post Title"
tags: [ml, notes]
math: true    # optional: enables LaTeX via KaTeX
---

Your content in Markdown. Inline math $x^2$, display math:

$$
f(x) = \sum_i w_i x_i
$$
```

Commit and push. Images can go in `assets/img/` and be referenced as
`![alt](/assets/img/figure.png)`.

## Add a paper

The Papers page shows "coming soon" until you add entries to `_data/papers.yml`. An example entry is commented out in that file. Your name is bolded automatically in author lists.

## Preview locally (optional)

```sh
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```
