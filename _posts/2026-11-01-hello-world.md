---
layout: post
title: "Hello, World"
tags: [meta]
math: true   # enables LaTeX rendering on this page
---

This is my first post. Every post is a Markdown file in `_posts/` named
`YYYY-MM-DD-title.md`. Commit it, push, and it shows up on the site.

## Math

Set `math: true` in the front matter to write LaTeX. Inline: $p_\theta(x)$.
Display:

$$
\mathcal{L}(\theta) = -\mathbb{E}_{x \sim \mathcal{D}} \left[ \log p_\theta(x) \right]
$$

## Code

```python
import torch

x = torch.randn(4, 8)
print(x.softmax(dim=-1).sum(dim=-1))
```

> Quotes look like this.

That's it. Delete this post when you write your own.
