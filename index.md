---
layout: default
title: About
---

<section class="intro">
  <img class="avatar" src="{{ '/assets/img/profile.svg' | relative_url }}" alt="{{ site.author.name }}">
  <div>
    <h1>{{ site.author.name }}</h1>
    <p class="subtitle">{{ site.author.role }}{% if site.author.affiliation != "" %} · {{ site.author.affiliation }}{% endif %}</p>
    {% include social-links.html %}
  </div>
</section>

Hi, I'm Sean. I studied Electrical and Computer Engineering at Seoul National University
and will begin my MS/PhD in AI next year. I write here about ideas I'm exploring
and things I've learned along the way.

## Recent posts

{% assign recent = site.posts | slice: 0, 5 %}
{% include post-list.html posts=recent %}
