---
layout: page
title: 留言
---
交换友链可以在评论区留言~

{% for friend in site.friends %}
<div class="card">
<div class="card-portrait"><img src="{{ friend.portrait }}"></div>
{{ friend.name }}{{ friend.src }}
</div>
{% endfor %}

- [wu-kan](https://wu-kan.github.io): 坎爷学长，在线教学，带我起飞

- [Max.C](https://437436999.github.io): 室友，一起快乐学习快乐打码~

- [Reborn](https://KomicaReborn.github.io): 计科三人组×1

- [林澈](https://52hert-z.github.io): 计科三人组×2

{% include valine.html %}
