---
layout: page
title: 周刊
permalink: /weekly/
---

这里是我的周刊栏目，不定期分享我在留学、语言学习、AI技术、工作和海外生活中的所见所闻和思考。

<ul class="post-list">
  {% for post in site.categories.weekly %}
    <li>
      <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
      {% if site.show_excerpts %}
        {{ post.excerpt }}
      {% endif %}
    </li>
  {% endfor %}
</ul>