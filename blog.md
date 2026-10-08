---
layout: default
title: Blog · Balaji Ramachandran
description: Coming soon!
permalink: /blog/
profile: false
---

<main class="page-layout blog-layout">
  <article class="content blog-content">
    <header class="blog-header">
      <p class="blog-kicker">Writing</p>
      <h1>:)</h1>
      <p>...</p>
    </header>

    {% if site.posts.size > 0 %}
      {% for post in site.posts %}
        <article class="blog-post-preview">
          <p class="blog-post-date">{{ post.date | date: "%B %-d, %Y" }}</p>
          <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
          {% if post.excerpt %}
            <p>{{ post.excerpt | strip_html | truncate: 220 }}</p>
          {% endif %}
          <a class="blog-read-more" href="{{ post.url | relative_url }}">Read more →</a>
        </article>
      {% endfor %}
    {% else %}
      <div class="blog-empty">
        <h2>...</h2>
        <p>...</p>
      </div>
    {% endif %}
  </article>
</main>
