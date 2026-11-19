---
layout: default
title: About
---

<section class="intro">
  <img class="avatar" width="1106" height="1422" src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="{{ site.author.name }}">
  <div>
    <h1>{{ site.author.name }}</h1>
    <p class="subtitle">{{ site.author.role }}{% if site.author.affiliation != "" %} @ {{ site.author.affiliation }}{% endif %}</p>
    {% include social-links.html %}
  </div>
</section>

Hi, I'm Sean. I'm studying Electrical and Computer Engineering at Seoul National University,
graduating in February 2027. In March, I'll join [M.IN.D Lab](http://mindlab-snu.notion.site/),
led by [Prof. Taesup Moon](https://scholar.google.com/citations?user=lQlioBoAAAAJ&hl=en),
as an MS/PhD student in Artificial Intelligence.

I write about my research, projects, and ideas that help me make sense of the world.

## Recent posts

{% assign recent = site.posts | slice: 0, 5 %}
{% include post-list.html posts=recent %}
