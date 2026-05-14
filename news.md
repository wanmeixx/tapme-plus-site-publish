---
layout: page
title: News
subtitle: TapMe.plus release notes and announcements.
permalink: /news/
---

{% assign news_items = site.news | sort: "date" | reverse %}

<ul class="posts-list list-unstyled" role="list">
{% for item in news_items %}
  <li class="post-preview">
    <article>
      <a href="{{ item.url | relative_url }}">
        <h2 class="post-title">{{ item.title }}</h2>
        {% if item.subtitle %}
          <h3 class="post-subtitle">{{ item.subtitle }}</h3>
        {% endif %}
      </a>
      <p class="post-meta">{{ item.date | date: site.date_format }}</p>
      <div class="post-entry">
        {{ item.excerpt | strip_html | truncatewords: 45 }}
        <a href="{{ item.url | relative_url }}" class="post-read-more">[Read&nbsp;More]</a>
      </div>
    </article>
  </li>
{% endfor %}
</ul>
