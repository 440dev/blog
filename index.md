---
layout: default
title: ホーム
---

## 投稿一覧

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span style="color: #666;"> - {{ post.date | date: "%Y年%m月%d日" }}</span>
    </li>
  {% endfor %}
</ul>