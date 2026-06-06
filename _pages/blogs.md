---
layout: default
title: "Blogs"
permalink: /blogs/
author_profile: false
---

<main class="page--wide" role="main">
  <h1>Blogs</h1>
  {% if site.posts.size > 0 %}
    <div class="works-list">
      {% for post in site.posts %}
        <article class="work-card">
          <div class="work-card__body">
            <a class="work-card__title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
            {% if post.date %}
              <p class="work-card__venue">{{ post.date | date: "%B %-d, %Y" }}</p>
            {% endif %}
            {% if post.excerpt %}
              <p class="work-card__summary">{{ post.excerpt | strip_html }}</p>
            {% endif %}
          </div>
        </article>
      {% endfor %}
    </div>
  {% else %}
    <div class="blog-empty">
      <p><strong>Coming soon.</strong></p>
      <p>Notes and research updates will appear here when new blog posts are added.</p>
    </div>
  {% endif %}
</main>
