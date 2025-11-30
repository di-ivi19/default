---
layout: default
title: Главная
---

# Добро пожаловать на мой сайт!

Это главная страница моего Jekyll-блога.

## Последние записи:
<ul>
{% for post in site.posts limit:3 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date_to_xmlschema }}">
      {{ post.date | date: "%d.%m.%Y" }}
    </time>
  </li>
{% endfor %}
</ul>
