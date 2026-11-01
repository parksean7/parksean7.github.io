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

Hi! I'm a graduate student working on **machine learning**. My research interests include
representation learning, large language models, and *[your topic here]*.

Before this, I studied [your background] at [your previous school]. I write here about
papers I'm reading, ideas I'm exploring, and things I've learned along the way.

Replace this text in `index.md` with your own introduction.

## Recent posts

{% assign recent = site.posts | slice: 0, 5 %}
{% include post-list.html posts=recent %}
