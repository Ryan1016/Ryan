---
layout: page
title: Do what you most want to do.
showtag:
- 程序设计
---
> "I'm loyal to nothing except the dream."   --Captain America

> "With great power comes great responsibility"   --Spider-man

> "I don't think that bolt of lightning struck you, Barry. I think it chose you." --The Flash

## 近期

{% for post in site.posts limit:5 %}

- [{{ post.title }}]({{ post.url }}), *{{ post.date | date_to_string }}*

{% if post.description %}

  > {{ post.description }}

{% endif %}

{% endfor %}

- [更多…](/archive)

{% for tag in page.showtag %}

## {{ tag }}

{% for post in site.tags[tag] %}

- [{{ post.title }}]({{ post.url }})

{% if post.description %}

  > {{ post.description }}

{% endif %}

{% endfor %}

{% endfor %}
