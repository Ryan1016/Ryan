---
layout: page
title: 心之所向便是光
showtag:
- 程序设计
- 数据结构
---

<h3 align="left">I'm loyal to nothing except the dream."</h3>
<h3 align="right">——Captain America</h3>

## 近期

{% for post in site.posts limit:5 %}

- [{{ post.title }}]({{ post.url }}), *{{ post.date | date_to_string }}*

{% if post.description %}

  > {{ post.description }}

{% endif %}

{% endfor %}

{% for post in site.posts limit:5 %}

<div class="postbox">[{{ post.title }}]({{ post.url }}), {{ post.date | date_to_string }}</div>

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