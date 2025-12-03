---
layout: home
title: "Главная"
description: "Добро пожаловать на мой сайт!"
---

# 👋 Привет, мир!

Добро пожаловать на мой сайт, созданный с помощью GitHub Pages и Jekyll.

## О чем этот сайт

Здесь я буду делиться:
- Своими мыслями и идеями
- Проектами и экспериментами
- Полезными находками из мира IT

## Недавние посты

{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%d.%m.%Y" }}
{% endfor %}

[Все посты →](/archive)

## Контакты

- 📧 Email: {{ site.email }}
- 🐙 GitHub: [{{ site.github_username }}](https://github.com/{{ site.github_username }})
{% if site.twitter_username %}
- 🐦 Twitter: [@{{ site.twitter_username }}](https://twitter.com/{{ site.twitter_username }})
{% endif %}

---

*Сайт создан с ❤️ и обновляется {{ site.time | date: "%d.%m.%Y" }}*
